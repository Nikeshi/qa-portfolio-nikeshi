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
