# SpringBoot-REST-API-Spring_Security

This is a Spring Boot CRUD application that provides basic operations for managing employees. The project includes Spring Security to secure the endpoints based on user roles (e.g., EMPLOYEE, MANAGER, ADMIN). The application also demonstrates integrating JPA with a MySQL database and securing the API using HTTP Basic Authentication.

# Features :-

CRUD Operations for Employee management :- 
1) Create
2) Read
3) Update
4) Delete Employees.

# Role-based Authorization with Spring Security:-

1) EMPLOYEE role for read access
2) MANAGER role for create, update, and partial update access
3) ADMIN role for delete access

# MySQL database for storing user credentials and employee information.

# Spring Boot with Spring Security for securing the endpoints.

# Technologies Used:-
1) Spring Boot
2) Spring Security
3) Spring Data JPA
4) MySQL
5) Hibernate
6) HTTP Basic Authentication

# Prerequisites:-
Before running the project, ensure that you have:
1) Java 17 or later installed
2) MySQL server running
3) A MySQL database for user and employee management

# API Endpoints
GET /api/employees: Get a list of all employees (Accessible by EMPLOYEE role)

GET /api/employees/{employeeId}: Get details of a specific employee (Accessible by EMPLOYEE role)

POST /api/employees: Add a new employee (Accessible by MANAGER role)

PUT /api/employees: Update an existing employee (Accessible by MANAGER role)

PATCH /api/employees/{employeeId}: Partially update an employee (Accessible by MANAGER role)

DELETE /api/employees/{employeeId}: Delete an employee (Accessible by ADMIN role)

# Security
* The API uses Spring Security to enforce role-based access control. Users are assigned roles (EMPLOYEE, MANAGER, ADMIN) that determine which API operations they can access.
* HTTP Basic Authentication is used to authenticate users.
* Modify the roles and users in the members and roles tables in MySQL to manage authentication.
