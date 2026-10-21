# Student Management System

CRUD web app built with Spring Boot, Spring Data JPA, Thymeleaf and MySQL.

Features: add, view, edit and delete students.

## Run locally

1. Install Java 17+ and MySQL, then create the database: CREATE DATABASE vedant;
2. Run: DB_PASSWORD='your_password' ./mvnw spring-boot:run
3. Open http://localhost:8080/students

## Run with Docker

    docker build -t student-management .
    docker run -p 8080:8080 -e SPRING_DATASOURCE_URL=jdbc:mysql://host.docker.internal:3306/vedant -e SPRING_DATASOURCE_USERNAME=root -e SPRING_DATASOURCE_PASSWORD='your_password' student-management
