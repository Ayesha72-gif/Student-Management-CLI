# Student Management CLI
## Software Requirements Specification (SRS)

### 1. Project Overview

Student Management CLI is a command-line application developed using Python. It allows users to manage student records through a terminal interface.

The application will allow users to add, view, update, delete, and search student records. All student information will be stored in a JSON file so that records remain available after the application is closed.

### 2. Project Objectives

- Develop a simple student management system using Python.
- Practice clean and modular code.
- Implement CRUD operations.
- Learn file handling using JSON.
- Apply input validation and error handling.
- Write and execute test cases.

### 3. Scope of the Project

In Scope:
- Add a new student.
- View all students.
- Search for a student by ID.
- Update student information.
- Delete a student record.
- Store and retrieve records using JSON.
- Validate user input.
- Handle common application errors.

Out of Scope:
- User authentication and login.
- Graphical user interface (GUI).
- Database integration (SQLite/PostgreSQL).
- Online student registration.
- Multiple user roles.

### 4. Target User

The application is designed for a single local user who wants to manage student records through a command-line interface.

### 5. Technology Stack

| Technology | Purpose |
|---|---|
| Python | Application development |
| JSON | Data storage |
| VS Code | Code editor |
| Git | Version control |
| GitHub | Project hosting |
| Pytest | Automated testing |

### 6. Student Data Fields

Each student record will contain:

| Field | Description | Validation |
|---|---|---|
| Student ID | Unique student identifier | Required and unique |
| Full Name | Student's complete name | Required, not empty |
| Age | Student's age | Required, positive integer |
| Email | Student's email address | Required, valid format |
| Course | Student's enrolled course | Required, not empty |

### 7. Functional Requirements

FR-01: Add Student

The system shall allow the user to add a new student by entering the student's ID, full name, age, email, and course.

FR-02: View All Students

The system shall display all student records currently stored in the application.

FR-03: Search Student

The system shall allow the user to search for a student using their unique Student ID.

FR-04: Update Student

The system shall allow the user to update the information of an existing student.

FR-05: Delete Student

The system shall allow the user to delete an existing student record using the Student ID.

FR-06: Save Student Records

The system shall save student records in a JSON file whenever data is added, updated, or deleted.

FR-07: Load Student Records

The system shall load previously saved student records when the application starts.

FR-08: Input Validation

The system shall validate user inputs and reject invalid or incomplete information.

FR-09: Error Handling

The system shall display meaningful error messages when an operation fails.

### 8. Non-Functional Requirements

NFR-01: Usability

The application shall provide a simple and understandable command-line menu.

NFR-02: Reliability

The application shall preserve saved student records when it is closed and restarted.

NFR-03: Maintainability

The code shall be divided into separate modules according to their responsibilities.

NFR-04: Data Integrity

The application shall prevent duplicate Student IDs and avoid overwriting existing records accidentally.

NFR-05: Error Management

The application shall handle invalid input and file-related errors without unexpected crashes.

### 9. User Stories

| ID | User Story |
|---|---|
| US-01 | As a user, I want to add a student so that I can store their information. |
| US-02 | As a user, I want to view all students so that I can see stored records. |
| US-03 | As a user, I want to search for a student so that I can find their information quickly. |
| US-04 | As a user, I want to update a student so that I can correct their information. |
| US-05 | As a user, I want to delete a student so that I can remove unnecessary records. |
| US-06 | As a user, I want my records saved so that I do not lose data after closing the application. |

### 10. Acceptance Criteria

The project will be considered successful when:

- The user can successfully add a valid student.
- Duplicate Student IDs are rejected.
- All saved student records can be viewed.
- A student can be searched using their ID.
- Existing student information can be updated.
- A student can be deleted.
- Changes are saved in the JSON file.
- Previously saved records load when the application restarts.
- Invalid input is handled with meaningful messages.
- The application passes its planned test cases.

### 11. Project Limitations

- The application will run locally on a computer.
- Only one user will manage the records.
- Data will be stored in a JSON file instead of a database.
- The application will not provide a graphical interface.

### 12. Future Improvements

The application may later be extended with:

- SQLite or PostgreSQL database.
- Django REST Framework API.
- Web-based graphical interface.
- User authentication.
- Student attendance management.
