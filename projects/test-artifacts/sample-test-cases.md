# 🔐 Reset Password – Test Cases

## Overview
This document contains manual test cases for the **Reset Password** functionality.  
The scenarios cover **functional, validation, usability, and security** aspects to ensure a reliable and secure password recovery process.

---

## TC_RP_001 – Reset Password with Valid Registered Email
**Precondition:** User has a registered email address  

**Steps:**
1. Navigate to the Login page  
2. Click on **Forgot Password**  
3. Enter a valid registered email address  
4. Click **Submit**

**Expected Result:**  
- A success message is displayed  
- A password reset email is sent to the registered email address

---

## TC_RP_002 – Reset Password with Unregistered Email
**Steps:**
1. Navigate to Forgot Password page  
2. Enter an unregistered email address  
3. Click **Submit**

**Expected Result:**  
- Appropriate error or generic message is displayed

---

## TC_RP_003 – Submit Reset Password with Empty Email Field
**Steps:**
1. Leave the email field empty  
2. Click **Submit**

**Expected Result:**  
- Validation message is displayed indicating email is required

---

## TC_RP_004 – Reset Password with Invalid Email Format
**Steps:**
1. Enter an invalid email format (e.g., `user@com`)  
2. Click **Submit**

**Expected Result:**  
- Email format validation message is displayed

---

## TC_RP_005 – Open Reset Password Link from Email
**Precondition:** Reset password email is received  

**Steps:**
1. Open the reset password email  
2. Click on the reset password link

**Expected Result:**  
- User is redirected to the Reset Password page

---

## TC_RP_006 – Use Expired Reset Password Link
**Steps:**
1. Open the reset password link after the expiry time  
2. Attempt to reset the password

**Expected Result:**  
- Expired link message is displayed  
- Option to request a new reset link is provided

---

## TC_RP_007 – Use Reset Password Link More Than Once
**Steps:**
1. Successfully reset the password using the link  
2. Attempt to reuse the same reset link

**Expected Result:**  
- Error message is displayed  
- User is prompted to request a new reset link

---

## TC_RP_008 – Reset Password with Valid New Password
**Steps:**
1. Enter a valid new password  
2. Enter the same password in the Confirm Password field  
3. Click **Submit**

**Expected Result:**  
- Password is reset successfully  
- User is redirected to the Login page

---

## TC_RP_009 – Password and Confirm Password Do Not Match
**Steps:**
1. Enter different values in Password and Confirm Password fields  
2. Click **Submit**

**Expected Result:**  
- Validation message indicating password mismatch is displayed

---

## TC_RP_010 – New Password Does Not Meet Policy Requirements
**Steps:**
1. Enter a password that does not meet policy requirements  
   (e.g., less than 8 characters, no special character)  
2. Click **Submit**

**Expected Result:**  
- Password policy validation message is displayed

---

## TC_RP_011 – Verify Old Password Is Invalid After Reset
**Steps:**
1. Reset the password successfully  
2. Attempt to log in using the old password

**Expected Result:**  
- Login fails using the old password

---

## TC_RP_012 – Login with New Password After Reset
**Steps:**
1. Log in using the newly reset password

**Expected Result:**  
- User is logged in successfully

---

## TC_RP_013 – Reset Password Using Different Browser or Device
**Steps:**
1. Request a reset password link  
2. Open the reset link on a different browser or device

**Expected Result:**  
- Reset Password page opens successfully

---

## TC_RP_014 – Security: Do Not Reveal Account Existence
**Steps:**
1. Enter any email address (registered or unregistered)  
2. Click **Submit**

**Expected Result:**  
- Generic message displayed (e.g., “If an account exists, a reset link has been sent”)
