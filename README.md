# Spring Boot API CRUD with Database
This is a simple Spring Boot application implementing CRUD operations with a MySQL database. It provides an API to manage subscription data, such as adding, updating, retrieving, and deleting subscriber details.

# Features
- CRUD operations: Create, Read, Update, Delete subscription records.
- RESTful API: Exposes endpoints to interact with the subscription database.
- MySQL Database Integration: Uses MySQL to store subscriber information.

# Technologies Used
- Spring Boot: Backend framework for building Java applications.
- MySQL: Relational database for storing subscription data.
- Postman: For testing the REST API.

# Prerequisites
- Java: JDK 11 or higher.
- Maven: Build tool for the project.
- MySQL: A running MySQL instance.

Setting Up the Project
1. Clone the Repository
   - Clone this repository to your local machine:
```
git clone https://github.com/RaamTechLead-DSAI/Spring-Boot-API-CRUD-DB.git
cd Spring-Boot-API-CRUD-DB

2. Set Up MySQL Database
- Install MySQL and start the MySQL server.
- Create a database for the application:
`CREATE DATABASE subscription_management;`

3. Configure the application.properties file in src/main/resources/ with your MySQL connection details:
```
spring.datasource.url=jdbc:mysql://localhost:3306/subscription_management
spring.datasource.username=<your_username>
spring.datasource.password=<your_password>
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

Make sure to replace <your_username> and <your_password> with your actual MySQL credentials.

4. Build and Run the Application
Use Maven to build and run the application:
```
mvn clean install
mvn spring-boot:run

The application will start on http://localhost:8080.

# Testing the API with Postman
1. Import Collection
You can import the provided Postman collection into Postman. This collection includes all the API requests that correspond to the CRUD operations.

2. Example Requests
- GET All Subscribers:
   - URL: http://localhost:8080/api/subscribers
   - Method: GET
- GET Subscriber by ID:
   - URL: http://localhost:8080/api/subscribers/{id}
   - Method: GET
- POST Create Subscriber:
   - URL: http://localhost:8080/api/subscribers
   - Method: POST

# Spring Boot CRUD API with MySQL Database

## Overview

This repository contains a Spring Boot application implementing a CRUD (Create, Read, Update, Delete) API connected to a MySQL database. The application is designed to manage subscriber information, such as name, email, and subscription status.

## Project Structure

- **Controller**: Manages the API endpoints for subscription-related actions.
- **Service**: Contains the business logic for managing subscriptions.
- **DAO**: Provides data access methods for interacting with the database.
- **Entity**: Defines the `Subscription` entity mapped to the database.

## Prerequisites

1. **Java 11 or higher**
2. **Maven**
3. **MySQL database**

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/RaamTechLead-DSAI/Spring-Boot-API-CRUD-DB.git
cd Spring-Boot-API-CRUD-DB

