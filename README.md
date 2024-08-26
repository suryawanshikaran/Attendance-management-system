# Attendance-management-system

• Classroom Endpoints:

	• GET /api/classrooms: Get all classrooms.
	• GET /api/classrooms/{id}: Get a specific classroom by ID.
	• POST /api/classrooms: Create a new classroom.
	• PUT /api/classrooms/{id}: Update an existing classroom.
	• DELETE /api/classrooms/{id}: Delete a classroom by ID.

• Class Schedule Endpoints:

	• GET /api/classSchedules: Get all class schedules.
	• GET /api/classSchedules/{id}: Get a specific class schedule by ID.
	• POST /api/classSchedules: Create a new class schedule.
	• PUT /api/classSchedules/{id}: Update an existing class schedule.
	• DELETE /api/classSchedules/{id}: Delete a class schedule by ID.

• Course Endpoints:

	• GET /api/courses: Get all courses.
	• GET /api/courses/{id}: Get a specific course by ID.
	• POST /api/courses: Create a new course.
	• PUT /api/courses/{id}: Update an existing course.
	• DELETE /api/courses/{id}: Delete a course by ID.

• Department Endpoints:

	• GET /api/departments: Get all departments.
	• GET /api/departments/{id}: Get a specific department by ID.
	• POST /api/departments: Create a new department.
	• PUT /api/departments/{id}: Update an existing department.
	• DELETE /api/departments/{id}: Delete a department by ID.

• Faculty Endpoints:

	• GET /api/faculties: Get all faculties.
	• GET /api/faculties/{id}: Get a specific faculty by ID.
	• POST /api/faculties: Create a new faculty.
	• PUT /api/faculties/{id}: Update an existing faculty.
	• DELETE /api/faculties/{id}: Delete a faculty by ID.

• Subject Endpoints:

	• GET /api/subjects: Get all subjects.
	• GET /api/subjects/{id}: Get a specific subject by ID.
	• POST /api/subjects: Create a new subject.
	• PUT /api/subjects/{id}: Update an existing subject.
	• DELETE /api/subjects/{id}: Delete a subject by ID.

**Brief Overview of the Project:**

• The Classroom Management System is a web-based application designed to streamline faculty management and course scheduling within educational institutions.

**Objectives and Goals:**

• Provide efficient course scheduling and faculty management tools.
• Enhance communication between faculty, administrators, and students.

**Scope of the Project:**

• The project includes features such as user authentication, course scheduling, and faculty profile management. It excludes integration with external systems, advanced analytics, and support for non-academic events.

**_---Project Structure---_**


**Overview of Project Architecture:**

• The project follows a layered architecture pattern, with distinct layers for handling different aspects of functionality and data management.

**Layers Description:**

1. Controller Layer: 

  • Responsible for handling incoming HTTP requests, processing them, and returning appropriate responses. Controllers act as the entry point to the application and delegate business logic to the service layer.

2. Service Layer: 

  • Acts as an intermediary between the controller and the data access layer (DAO). It contains business logic and orchestrates interactions between different parts of the application. Services handle tasks such as validation, data manipulation, and transaction management.

3. DAO (Data Access Object) Layer:

  • Responsible for interacting with the database and performing CRUD (Create, Read, Update, Delete) operations on the underlying data. DAOs abstract away the details of database interactions and provide a clean interface for the service layer to work with.

**Responsibilities of each layer:**

Controller Layer:
Handle incoming HTTP requests.
Validate request parameters and payload.
Invoke appropriate methods in the service layer.
Format and return HTTP responses.

Service Layer:
Implement business logic and rules.
Coordinate interactions between controllers and DAOs.
Perform data manipulation and transformation.
Manage transactions and ensure data integrity.

DAO Layer:
Provide CRUD operations for accessing and modifying data.
Translate database queries and commands into appropriate SQL statements.
Handle database transactions and connections.
Abstract away database-specific details from the service layer.


_**---Modules---**_

**1. Class Management Module:**

• Description of functionality: This module handles the management of classes, including creating, editing, and deleting class information. It also facilitates assigning classrooms, subjects, and faculty to classes.

• List of features:
Create, edit, and delete class information.
Assign classrooms, subjects, and faculty to classes.
View class schedules and associated details.

**2. Faculty Management Module:**

• Description of functionality: This module focuses on managing faculty members within the educational institution. It includes features for adding new faculty, updating their information, and assigning courses and departments.

• List of features:
Add, update, and delete faculty profiles.
Assign courses and departments to faculty members.
View faculty details and their associated courses.

**3. Course Management Module:**

• Description of functionality: This module is responsible for managing academic courses offered by the institution. It allows administrators to create new courses, update existing ones, and assign faculty and departments to each course.

• List of features:
Create, update, and delete course information.
Assign faculty and departments to courses.
View course details and associated faculty and departments.

**4. Department Management Module:**

• Description of functionality: This module handles the management of academic departments within the institution. It enables administrators to create new departments, update their details, and assign faculty members and courses to each department.

• List of features:
Create, update, and delete department information.
Assign faculty members and courses to departments.
View department details and associated faculty members and courses.

**5. Subject Management Module:**

• Description of functionality: This module focuses on managing academic subjects taught within the institution. It allows administrators to add new subjects, update their details, and assign them to courses and departments.

• List of features:
Add, update, and delete subject information.
Assign subjects to courses and departments.
View subject details and associated courses and departments.




_**---Type of Users of a Project---**_

**1. Admin:**

• Roles and Responsibilities:

    • Manage system settings and configurations.
    • Create and manage user accounts.
    • Manage class schedules, faculty information, course details, and department information.
    • Generate reports and analytics.
    • Handle system maintenance and updates.

• Access Levels:

    • Full access to all modules and features of the system.
    • Can perform administrative tasks such as user management, data management, and system configuration.

**2. Faculty:**

• Roles and Responsibilities:
    
    • Manage course schedules, assignments, and assessments.
    • Communicate with students regarding course materials and assignments.
    • Monitor student progress and grades.

• Access Levels:

    • Limited access to course management and student information.
    • Can view and update course details and student grades.

**3. Student:**

• Roles and Responsibilities:

    • Attend classes and participate in course activities.
    • Submit assignments, quizzes, and exams.
    • View course materials and announcements.
    • Monitor their own grades.

• Access Levels:

    • Limited access to personal academic information and course materials.
    • Can view course schedules, assignments, and grades.
