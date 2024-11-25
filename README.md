# Spring Boot CRUD Application

## About the Project

This project is a **Spring Boot-based CRUD application** designed to manage **Categories** and **Products**. It incorporates the following features:

- **RESTful APIs** to perform CRUD operations.
- **One-to-Many Relationship**: A category can contain multiple products.
- **Pagination Support**: Implements server-side pagination for both categories and products.
- **Database Integration**: Configured with **MySQL** using **JPA** and **Hibernate**.
- **Annotation-based Configuration**: No XML configurations.

---

## Key Features

- **CRUD Operations** for managing categories and products.
- **Relational Database**: Uses MySQL for data persistence.
- **Pagination**: Supports server-side pagination for efficient data retrieval.
- **Clean Architecture**:
  - **Controller Layer**: Handles HTTP requests and responses.
  - **Service Layer**: Contains the application's business logic.
  - **Repository Layer**: Manages database operations with JPA.

---

## Technologies Used

- **Java 17**
- **Spring Boot**
- **Spring Data JPA**
- **Hibernate**
- **MySQL**
- **Postman** for API testing
- **Maven** for build automation

---

## Folder Structure

```plaintext
spring-boot-crud-app/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── com/
│   │   │   │   ├── example/
│   │   │   │   │   ├── controller/
│   │   │   │   │   │   ├── CategoryController.java                // REST controller for Category
│   │   │   │   │   │   ├── ProductController.java                 // REST controller for Product
│   │   │   │   │   ├── entity/
│   │   │   │   │   │   ├── Category.java                          // Entity class for Category
│   │   │   │   │   │   ├── Product.java                           // Entity class for Product
│   │   │   │   │   ├── repository/
│   │   │   │   │   │   ├── CategoryRepository.java                // Repository for Category
│   │   │   │   │   │   ├── ProductRepository.java                 // Repository for Product
│   │   │   │   │   ├── service/
│   │   │   │   │   │   ├── CategoryService.java                   // Service layer for Category
│   │   │   │   │   │   ├── ProductService.java                    // Service layer for Product
│   │   │   │   │   ├── SpringBootCrudApplication.java             // Main Application
│   │   │   │   │   ├── config/
│   │   │   │   │   │   ├── AppConfig.java                         // Additional configurations
│   │   ├── resources/
│   │   │   ├── application.properties                             // Database & server configurations
