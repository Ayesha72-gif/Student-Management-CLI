# Student Management CLI
## Test Case Document

### 1. Add Student Module

| Test ID | Test Scenario | Preconditions | Test Data | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|
| TC-01 | Add a student with valid information | Application is running | ID: 101, Name: Ali, Age: 20, Email: ali@gmail.com, Course: BSCS | Student should be added successfully | | Not Executed |
| TC-02 | Add a student with an existing ID | Student ID 101 already exists | ID: 101 | System should reject duplicate ID | | Not Executed |
| TC-03 | Add a student with an empty name | Application is running | Name: Empty | System should display validation error | | Not Executed |
| TC-04 | Add a student with invalid age | Application is running | Age: -5 | System should reject invalid age | | Not Executed |
| TC-05 | Add a student with invalid email | Application is running | Email: ali123 | System should reject invalid email | | Not Executed |
| TC-06 | Add a student with missing information | Application is running | Course: Empty | System should display validation error | | Not Executed |

### 2. View All Students Module

| Test ID | Test Scenario | Preconditions | Test Data | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|
| TC-07 | View all saved students | At least one student exists | Existing student records | All student records should be displayed | | Not Executed |
| TC-08 | View students when no records exist | No student records exist | Empty records | System should display a message that no students are available | | Not Executed |

### 3. Search Student Module

| Test ID | Test Scenario | Preconditions | Test Data | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|
| TC-09 | Search for an existing student | Student ID 101 exists | ID: 101 | Matching student details should be displayed | | Not Executed |
| TC-10 | Search for a non-existing student | Application is running | ID: 999 | System should display Student Not Found | | Not Executed |
| TC-11 | Search using an empty ID | Application is running | ID: Empty | System should display validation error | | Not Executed |

### 4. Update Student Module

| Test ID | Test Scenario | Preconditions | Test Data | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|
| TC-12 | Update an existing student's information | Student ID 101 exists | Name: Ahmed | Student information should be updated successfully | | Not Executed |
| TC-13 | Update a non-existing student | Application is running | ID: 999 | System should display Student Not Found | | Not Executed |
| TC-14 | Update with invalid age | Student ID 101 exists | Age: -10 | System should reject invalid age | | Not Executed |
| TC-15 | Update with invalid email | Student ID 101 exists | Email: invalid-email | System should reject invalid email | | Not Executed |

### 5. Delete Student Module

| Test ID | Test Scenario | Preconditions | Test Data | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|
| TC-16 | Delete an existing student | Student ID 101 exists | ID: 101 | Student should be deleted successfully | | Not Executed |
| TC-17 | Delete a non-existing student | Application is running | ID: 999 | System should display Student Not Found | | Not Executed |
| TC-18 | Delete using an empty ID | Application is running | ID: Empty | System should display validation error | | Not Executed |

### 6. JSON File Storage Module

| Test ID | Test Scenario | Preconditions | Test Data | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|
| TC-19 | Save a new student record | Application is running | Valid student data | Student data should be saved in JSON file | | Not Executed |
| TC-20 | Load existing records | JSON file contains student records | Existing JSON data | Previously saved records should load successfully | | Not Executed |
| TC-21 | Start application without JSON file | JSON file does not exist | Missing file | Application should handle missing file safely and initialize empty records | | Not Executed |
| TC-22 | Load corrupted JSON file | JSON file contains invalid JSON | Corrupted JSON | Application should handle JSON decoding error safely | | Not Executed |
| TC-23 | Verify records after application restart | Student records have been saved | Existing records | Records should remain available after restarting application | | Not Executed |

### 7. Application Menu Module

| Test ID | Test Scenario | Preconditions | Test Data | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|
| TC-24 | Select a valid menu option | Application is running | Option: 1 | Selected operation should execute | | Not Executed |
| TC-25 | Select an invalid menu option | Application is running | Option: 9 | System should display Invalid Choice | | Not Executed |
| TC-26 | Exit the application | Application is running | Exit option | Application should close safely | | Not Executed |

### 8. Test Execution Summary

| Total Test Cases | Passed | Failed | Not Executed |
|---|---|---|---|
| 26 | 0 | 0 | 26 |

Note: Actual Result and Status will be updated after implementation and test execution.
