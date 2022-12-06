## Test Suite
|Test Case| Desc | Steps |
|---------|------|-------|
|TC-1| Navigate to homepage without entering credentials | Navigate to homepage.html without entering credentials. Verify redirect to login.html |
|TC-2| Login with correct credentials | Type username as "username" and password  as "password". Press login. Verify on homepage for username | 
|TC-3| Login with correct username and incorrect password | Type username as "username" and password  as "notthepassword". Press submit. Verify message says "login has failed." |
|TC-4| Login with invalid username | Type username as "nottheusername and password as "notthepassword". Press submit. Verify message says "login has failed." |
|TC-5| Login with username and password fields blank | Make sure username and password fields are blank. Press login. Verify message says "login has failed." |


## Defect Report
|Defect | Desc | Severity | Priority | Steps to reproduce |
|-------|------|----------|----------|--------------------|
|DEF-1   |Popup message says "username incorrect" instead of "login has failed" | low | low | Login with a correct username and incorrect password |
|DEF-2 | Popup message says "password incorrect" instead of "login has failed" | low | low | Login with an invalid username and any password |
|DEF-3 | Popup message says "password incorrect" instead of "login has failed" | low | low | Leave username and password fields blank and press submit |

## Requirements Traceability Matrix
|Requirement| Test Cases | Status | Defects |
|-----------|------------|--------|---------|
|Users should only be able to access the homepage if they enter correct login credentials on the login page | TC-1, TC-2 | TC-1 PASS, TC-2 PASS | |
|Users should see a generic message saying login has failed if they provide the wrong credentials | TC-3, TC-4, TC-5 | TC-3 FAIL, TC-4 FAIL, TC-5 FAIL | DEF-1, DEF-2, DEF-3 |  |