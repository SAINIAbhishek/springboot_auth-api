# Spring Boot Authentication & Authorization Backend Project (Learning project)

A scalable and well-structured Spring Boot backend project designed to handle the scale and complexity of an application. It is designed while taking into consideration the different environments.

The project structure follows the best practices and conventions of a Spring Boot application.

Following are the features of this project:

- **Role-Based Access Control**: enhances security by granting or restricting permissions based on user roles, allowing fine-grained access management.
- **User Verification**: Send the verification email to the user used at the time of registration.

## Stacks:
- Spring Boot
- Spring Security
- Java Mail
- Email verification with expiry
- PostgreSQL

## Testing the Routes and Functionality

To test the routes and functionality of this API you can use tool like **POSTMAN**.

- Install Postman if you haven't already.
- Start the backend server, making sure it's running on the correct port.

## Java Transaction API (JTA)

The Java Transaction API (JTA) is a Java Enterprise Edition (Java EE) standard API that provides a way to manage transactions across multiple resources in a distributed environment. 
It allows you to coordinate transactions across multiple transactional resources such as databases (via JDBC), message queues (via JMS), and other enterprise information systems.

## hibernate.ddl-auto

- **Validate**: Hibernate validates that the existing schema matches the expected schema. It does not make any changes to the database schema.
- **Update**: Hibernate automatically updates the database schema to match the entity mappings. It adds new tables, columns, and constraints but does not drop existing schema objects.
- **Create**: Hibernate creates the database schema from scratch when the application starts. It drops and recreates all tables, indexes, constraints, etc., losing any existing data.
- **Create-drop**: Hibernate creates the database schema when the application starts, like create. However, it also drops the schema when the SessionFactory is closed (typically when the application shuts down), which is useful for development and testing to reset the database state.
- **None**: Hibernate does not perform any automatic schema management. It expects the application to manage the database schema manually.

## jpa.open-in-view

In the **development environment**, enabling spring.jpa.open-in-view can be convenient for debugging and development purposes. It allows lazy loading of entity relationships to be managed 
automatically, which can simplify development by reducing the need for explicit transaction management in certain scenarios.

In the **production environment**, it's generally recommended to disable spring.jpa.open-in-view. This is crucial for optimizing performance and minimizing database access overhead, 
especially in applications handling a large volume of requests.