## Test Suite
|Test Case| Desc | Steps |
|---------|------|-------|
|TC-1| Complete form as intended. | Enter first and last name at the beginning of the document. Enter capitalized initials at the end of the document. Select checkbox at the top of the page, and click Continue. Verify popup saying "The pact is sealed." |
|TC-2| Complete form except for first and last name at the beginning of the document. | Leave first and last name fields blank. Enter capitalized initials at the end of the document. Verify document cannot be submitted. |
|TC-3| Complete form without capitalizing initials at the end of the document. | Enter first and last name at the beginning of the document. Enter uncapitalized initials at the end of the document | Verify document cannot be submitted. |
|TC-4| Complete form, then erase fields before pressing Continue | Fill out first and last name at the beginning of the document. Enter capitalized initials at the end of the document. Erase fields. Verify document cannot be submitted. |
|TC




## Defect Report
|Defect | Desc | Severity | Priority | Steps to reproduce |
|-------|------|----------|----------|--------------------|
|DEF-1 | Document can be submitted with incorrect data | high | high | Fill out form correctly, then modify text inputs in any way desired. The document can still be submitted |


## Requirements Traceability Matrix
|Requirement| Test Cases | Status | Defects |
|-----------|------------|--------|---------|
| Users should not be able to continue until they have read the entire legal document | TC-4 | TC-4 FAIL | DEF-1 |
| Users must provide their first and last name at the start of the document | TC-1, TC-2, TC-4 | TC-1 PASS, TC-3 PASS, TC-4 FAIL | DEF-1 |
Users must initial the document at the end with their first and last initials capitalized | TC-1, TC-3, TC-4 | TC-1 PASS, TC-3 PASS, TC-4 FAIL | DEF-1 |