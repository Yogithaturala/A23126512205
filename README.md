# Logging Middleware

## Overview
This project is a Spring Boot-based Logging Middleware that handles authentication, generates logs, and sends them securely to a remote server using Bearer token authorization.

## Features
- Spring Boot application setup
- Authentication with external server
- Bearer token-based authorization
- Custom Logging Service
- Automatic startup log generation
- REST API integration
- Log submission tracking with response handling

## Tech Stack & Tools Used

### Java 17+
Used as the core programming language because it provides strong object-oriented features, reliability, and wide support for backend development.

### Spring Boot
Used to build the backend application quickly with minimal configuration. It simplifies dependency management, embedded server setup, and REST API creation.

### Spring Framework
Used for dependency injection and modular architecture, making the application loosely coupled and easier to maintain.

### Maven
Used as the build and dependency management tool. It helps manage project dependencies, build lifecycle, and ensures consistent project compilation.

### REST APIs
Used for communication between the application and external server for sending logs and receiving responses.

### IntelliJ IDEA
Used as the development environment for writing, testing, and debugging the Spring Boot application efficiently.

## Project Structure
src/main/java/com/yogitha/logging_middleware

├── LoggingMiddlewareApplication.java  
├── logging/  
│   └── LoggingService.java  
├── dto/  
│   └── LogRequest.java  
├── utils/  
│   └── StartupRunner.java  

src/main/resources/  
└── application.properties  

## How It Works
1. Application starts using Spring Boot  
2. Authentication token is generated/retrieved  
3. LoggingService creates structured logs  
4. Logs are sent to remote server using Bearer token  
5. StartupRunner triggers automatic log generation on startup  

## Sample Response
```json
{"logID":"20b150d1-8a8f-443e-b5b9-2a5e3ea97b6c","message":"log created successfully"}
