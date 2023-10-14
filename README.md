# fullstack-employee-manager-app-backend
Employee Management App Backend with CRUD Operations

This is a Java, SQL, and Spring Boot backend for an employee management application that enables one to add, edit, delete, and view employees. The backend features a REST API that can be used by the frontend Angular application to perform CRUD operations on employee data.

The backend also features a database to store employee data. The database is implemented using SQL and is compatible with all major relational database management systems (RDBMS), such as MySQL, PostgreSQL, and Oracle.

The backend is built using Spring Boot, which is a framework that makes it easy to develop Spring-based applications. Spring Boot provides a number of features that simplify the development process, such as automatic configuration and dependency injection.

The backend exposes the following CRUD endpoints:

/employees - Get a list of all employees
/employees/{id} - Get the details of a specific employee
/employees - Create a new employee
/employees/{id} - Update the details of a specific employee
/employees/{id} - Delete a specific employee
To use the backend, you can make GET, PUT, DELETE, and POST requests to the above endpoints using any HTTP client, such as curl or Postman.

Here are some examples of how to use the CRUD endpoints:

To get a list of all employees, you can make the following request:
curl http://localhost:8080/employees
To create a new employee, you can make the following request:
curl -X POST http://localhost:8080/employees -H "Content-Type: application/json" -d '{
    "name": "John Doe",
    "age": 30,
    "department": "Engineering"
}'
To update the details of an existing employee, you can make the following request:
curl -X PUT http://localhost:8080/employees/1 -H "Content-Type: application/json" -d '{
    "name": "Jane Doe",
    "age": 25,
    "department": "Sales"
}'
To delete an existing employee, you can make the following request:
curl -X DELETE http://localhost:8080/employees/1
