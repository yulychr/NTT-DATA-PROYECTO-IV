# NTT-DATA-PROYECTO-IV

## Descripcion

This project includes the implementation of two microservices that interact with relational databases: one for Customers and one for Accounts. These microservices are designed to manage customer information and their associated accounts efficiently, using microservices architecture principles.

## Features

**Unit Tests (JUnit):**
Unit tests have been implemented for all key methods of the main classes in the project. These tests ensure the correct functionality of the microservices, verifying the expected behaviors under different conditions.

**Mocks with Mockito:**
In those cases where it is necessary to simulate the behavior of external dependencies, such as interactions with the database, Mockito has been used to create mocks, guaranteeing a controlled and isolated testing environment.

**Code Coverage (JaCoCo):**
A code coverage report has been integrated using JaCoCo. This report allows you to evaluate the percentage of code covered by unit tests, providing detailed metrics on code quality and test effectiveness.

**Checkstyle Application:**
Checkstyle has been applied to the source code to ensure that the project follows best coding practices and maintains a consistent style, facilitating readability and maintainability of the code.

**SOLID Evaluation and Design Patterns:**
The code has been evaluated to ensure adherence to SOLID principles and design patterns have been implemented where appropriate. This improves the maintainability, extensibility and scalability of the system. In addition, areas for improvement have been identified and refactorings have been proposed to optimize the code structure.

## Implemented Microservices

###Customer Microservice:
This microservice manages the creation, list all customers, Get details of a customer by its ID, update and deletion in the database.

###Account Microservice:
This microservice manages customers' bank accounts, allowing operations such as account creation, deposits, withdrawals, account deletion, listing all accounts, and Getting details of an account by its ID.

**Complying with the following business rules**
1. Client Validations:
- Each client must have a unique ID.
- Deleting a client is not allowed if they have active accounts.
2. Bank Account Validations:
- The initial balance of an account must be greater than 0.
- You cannot make a withdrawal that leaves the balance in negative for savings accounts.
- Checking accounts may have an overdraft of up to -500.

## Technologies used

**- Java 17:** For the implementation of microservices. 
**- Spring Boot:** For the creation and management of microservices. 
**- JPA:** For managing data persistence in relational databases.
**- MySQL:** For the relational database used in the project.
**- Lombok:** For the automatic generation of getters, setters and other common methods in classes.
**- JUnit:** For unit testing. 
**- Mockito:** For creating mocks and isolated tests. 
**- JaCoCo:** For measuring code coverage. 
**- Checkstyle:** For code style control. 
**- Maven:** As a project dependency and construction manager

## Continuous Improvement

This project follows a continuous improvement approach, meaning that implementations are regularly reviewed and refactored to improve code quality, test coverage, and compliance with **SOLID** principles.

## Additional Notes
