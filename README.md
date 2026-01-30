```
QA-Tester-Portfolio-Nikeshi-Kiriwaththuduwa/
│
├── README.md
├── projects/
│ ├── firem.md
│ ├── bbb-recruitment.md
│ ├── bennets.md
│ └── knight-frank.md
├── test-artifacts/
│ ├── sample-test-cases.md
│ ├── sample-bug-reports.md
│ └── sample-test-plan.md
├── api-testing/
│ └── postman-summary.md
└── automation-learning/
│ └── automation-roadmap.md
``` 
# 👩‍💻 QA Tester Portfolio – Nikeshi Kiriwaththuduwa

Hi! I’m **Nikeshi**, a QA Tester with **2+ years of hands-on experience** in manual testing across mobile and web system-based applications.

I love finding issues before users do, exploring edge cases, and working closely with developers and product teams to deliver software that just works.  
I’m currently expanding my skills into automation testing and product operations, while keeping my focus on quality and organization.  

I enjoy turning tricky scenarios into clear test cases and helping teams release software with confidence..

---

## 🧪 Core Skills

**Testing Types**
- Manual Testing
- Functional & UI Testing
- Regression & End-to-End Testing
- Cross-Browser Testing
- API Testing
- Performance Testing
- Security Testing (Basic)

**Tools & Technologies**
- Jira
- Postman
- JMeter
- BrowserStack
- Agile / Scrum
- Zephyr

**Strengths**
- Strong analytical thinking
- Edge-case and negative testing mindset
- Clear bug documentation
- Cross-team collaboration
- Adaptability in fast-moving environments

---

## 📂 Project Experience

| Project | Domain | Highlights |
|------|------|-----------|
| FireM | Fire Alarm System | Critical system testing, edge cases |
| BBB | Recruitment Platform | Hiring workflows & filtering |
| Bennets | Fuel Distribution | Reliability & regression |
| Knight Frank | Property System | Admin workflows & reporting |
| &ShareApp | Mobile/Web Social Media Utility App |Enabled seamless one-tap social media handle sharing with reliable cross-platform performance and robust QA validation |

👉 Detailed project breakdowns are available in the **/projects** folder.

---

## 📑 Test Artifacts

- Sample Test Cases
- Sample Bug Reports (Jira-style)
- Sample Test Plan
- API Testing Summary (Postman)

📁 See **/test-artifacts** folder.

---

## 🤖 Automation Interest

While my primary experience is in manual QA, I am **passionate about automation testing** and actively learning how automation can improve regression coverage and efficiency.

📁 See **/automation-learning** folder.

---

## 📬 Contact

- **LinkedIn:**(https://www.linkedin.com/in/nikeshi-kiriwaththuduwa-a3740a293/)
- **Email:** (nikeshikiriwaththuduwa@gmail.com)

Thank you for reviewing my portfolio!
# 🔥 FireM – Fire Alarm System (Australia)

**Type:** Web-based Critical System  
**Role:** QA Tester  
**Environment:** QA, Staging, Production  

## What I Tested
- Alarm triggers and notifications
- System responses under different conditions
- User access and permissions
- UI behavior across browsers

## Testing Performed
- Manual testing
- Functional & UI testing
- Regression testing
- Cross-browser testing (BrowserStack)

## Tools Used
- Jira
- BrowserStack
- Google Docs

## QA Focus
- Edge-case and failure scenario testing
- Verifying fixes before release
- Close collaboration with developers
# 🧑‍💼 BBB – Recruitment & Candidate Filtering System

**Type:** Web Application  
**Domain:** Hiring & Recruiting  

## What I Tested
- Job posting workflows
- Candidate filtering logic
- Resume uploads and status changes

## Testing Performed
- Manual & functional testing
- Regression testing
- API testing (Postman)

## Why This Matters
This project gave me direct exposure to **recruiting workflows**, making me comfortable supporting admin and hiring-related operations.
# ⛽ Bennets – Fuel Distribution System (Australia)

## Testing Focus
- Functional workflows
- Data validation
- Regression before releases

## Tools
- Jira
- Manual test cases

## Key Takeaway
Worked on a reliability-critical system where accuracy and consistency were essential.
# 🏠 Knight Frank – Property Valuation System

## What I Tested
- Property data management
- Valuation report generation
- Admin workflows

## Testing Types
- Manual testing
- UI & functional testing
- Regression testing

## Collaboration
Worked closely with clients and developers to ensure smooth operational workflows.
# 🔗 &Share – Social Media Connection App

**Type:** Mobile/Web Social Media Utility App  
**Role:** QA Tester  
**Environment:** QA, Staging, Production  

## What I Tested
- Social media handle exchange functionality  
- Personalized card creation and sharing  
- Cross-platform connectivity  
- UI behavior across devices and browsers  

## Testing Performed
- Manual testing  
- Functional testing  
- UI testing  
- Performance testing (JMeter)  
- Cross-browser testing (BrowserStack)  
- Security testing (Quyles)  
- API testing (Postman)  
- Regression testing  
- End-to-end testing  

## Tools Used
- Jira  
- Postman  
- JMeter  
- BrowserStack  
- Quyles  

## QA Focus
- Edge-case and negative scenario testing  
- Ensuring seamless handle sharing across platforms  
- Verifying security and performance under load  
- Close collaboration with developers to validate fixes

# ✅ Sample Test Cases

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

# 🐞 Bug Report – Reset Password Functionality

## Bug ID
BUG_RP_001

## Title
Reset password link expires immediately after being generated

---

## Environment
- Application: Web Application  
- Environment: Production  
- Browser: Google Chrome (v latest)  
- OS: Windows 10  

---

## Severity
High

## Priority
High

---

## Description
When a user requests a password reset, the reset password link sent via email becomes invalid immediately upon opening, preventing the user from resetting their password.

---

## Preconditions
- User has a registered account  
- User has access to the registered email address  

---

## Steps to Reproduce
1. Navigate to the Login page  
2. Click on **Forgot Password**  
3. Enter a valid registered email address  
4. Click **Submit**  
5. Open the password reset email  
6. Click on the reset password link immediately

---

## Actual Result
- An error message is displayed stating that the reset password link is expired or invalid

---

## Expected Result
- The reset password link should remain valid for the configured expiration time  
- User should be redirected to the Reset Password page

---

## Frequency
100% (Occurs every time)

---

## Impact
- Users are unable to reset their passwords  
- High risk of user drop-off and support tickets  
- Impacts user access and trust

---

## Attachments
- Screenshot of error message  
- Email content showing reset link timestamp  

---

## Notes
- Issue reproduced across multiple attempts  
- No workaround available at the moment

# 🧾 Sample Test Plan

## Objective
Ensure application stability before release.

## Scope
- Functional testing
- Regression testing
- UI validation

## Tools
- Jira
- BrowserStack
# 🤖 Automation Learning & Passion

I am actively learning automation testing to complement my strong manual QA foundation.

## Current Focus
- Understanding what to automate vs what not to automate
- Learning automation concepts
- Exploring Selenium / Playwright basics
## Goal
Use automation to improve regression coverage while maintaining strong manual exploratory testing.


