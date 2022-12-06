## Test Suite
|Test Case| Desc | Steps |
|---------|------|-------|
|TC-1| Sign up with short username. | Enter "Abc1" as the username and "Abc123" as the password. Press submit button. Verify failure to sign up. |
|TC-2| Sign up with long username. | Enter "Abc12345678" as the username and "Abc123" as the password. Press submit button. Verify failure to sign up. |
|TC-3| Sign up with short password. | Enter "Abc123" as the username and "Abc1" as the password. Press submit button. Verify failure to sign up. |
|TC-4| Sign up with long password. | Enter "Abc123" as the username and "Abc12345678" as the password. Press submit button. Verify failure to sign up. |
|TC-5| Sign up with invalid password. | Enter "Abc123" as the username and "abcdef" as the password. Press submit button. Verify failure to sign up. |
|TC-6| Sign up with invalid username. | Enter "abcdef" as the username and "Abc123" as the password. Press submit button. Verify failure to sign up. |
|TC-7| Sign up with matching username and password. | Enter "Abc123" as the username and "Abc123" as the password. Press submit button. Verify failure to sign up. |
|TC-8| Sign up with valid and non-matching username and password of correct length | Enter "Mario123" as the username and "Luigi123" as the password. Press submit button. Verify successful signup. |



## Defect Report
|Defect | Desc | Severity | Priority | Steps to reproduce |
|-------|------|----------|----------|--------------------|
|DEF-1 | User is allowed to sign up with matching username and password | high | high | Enter the save valid string for username and password and press submit. |


## Requirements Traceability Matrix
|Requirement| Test Cases | Status | Defects |
|-----------|------------|--------|---------|
|Usernames and passwords must contain 6-10 characters | TC-1, TC-2, TC-3, TC-4 | TC-1 PASS, TC-2 PASS, TC-3 PASS, TC-4 PASS | |
|Usernames and passwords must contain a lowercase letter, an uppercase letter, and a number | TC-5, TC-6 | TC-5 PASS, TC-6 PASS | |
|Usernames must not match each other | TC-7 | TC-7 FAIL | DEF-1 |
|User is able to log in with valid username and password | TC-8 | TC-8 PASS | |