# API Java Spring H2 DB

A REST API built with Java Spring Boot and H2 Database, designed for lightweight development and testing.

## Overview

This project aims to achieve the following goals:
1. Create Spring Boot Project
2. Configure H2 Database
3. Create Domain Class (Entity) with JPA ORM
4. Perform Database Seeding
5. Retrieve Data with Pagination

## Technology Stack

- Java 21
- Spring Boot 4.0.3
- Spring Data JPA
- H2 Database (In-memory)
- Spring Web MVC
- Maven 3.6+

## Features

- RESTful API endpoints
- JPA entity mapping and database persistence
- H2 Console for interactive database management
- Maven build automation
- Comprehensive unit and integration testing setup
- Spring Boot starter dependencies for quick setup

## Project Structure

```
api-java-spring-h2-db/
├── src/
│   ├── main/
│   │   ├── java/              # Application source code
│   │   └── resources/         # Configuration files
│   └── test/                  # Test files
├── pom.xml                    # Maven configuration
├── mvnw / mvnw.cmd           # Maven wrapper scripts
└── README.md                  # Documentation
```

## Getting Started

### Prerequisites

- Java 21 or higher installed
- Maven 3.6 or higher (or use the included Maven wrapper)

### Installation

1. Clone the repository:
```
git clone https://github.com/nalugao/api-java-spring-h2-db.git
cd api-java-spring-h2-db
```

2. Build the project using Maven:
```
./mvnw clean install
```

For Windows:
```
mvnw.cmd clean install
```

3. Run the application:
```
./mvnw spring-boot:run
```

The application will start on http://localhost:8080

## Database Configuration

The H2 database is configured as an in-memory database, making it perfect for development and testing. No external database setup is required.

### H2 Console

Access the H2 Database Console at:
```
http://localhost:8080/h2-console
```

Default H2 Console Settings:
- Driver Class: org.h2.Driver
- JDBC URL: jdbc:h2:mem:testdb
- User Name: sa
- Password: (leave empty)

## Dependencies

### Core Dependencies

- spring-boot-starter-web: Web framework and REST support
- spring-boot-starter-data-jpa: ORM and database persistence
- spring-boot-h2console: Interactive H2 database console
- h2: In-memory relational database

### Test Dependencies

- spring-boot-starter-data-jpa-test: JPA testing utilities
- spring-boot-starter-webmvc-test: Web MVC testing support

## Building and Running

### Build the Project
```
./mvnw clean install
```

### Run Tests
```
./mvnw test
```

### Run the Application
```
./mvnw spring-boot:run
```

### Package as JAR
```
./mvnw clean package
```

## Maven Plugins

The project uses the Spring Boot Maven Plugin for building and running the application. This provides convenient goals for building and running Spring Boot applications directly from Maven.

## API Development

To develop your own API endpoints:

1. Create entity classes in src/main/java
2. Create repository interfaces extending JpaRepository
3. Create service classes for business logic
4. Create controller classes with REST endpoints

Example controller structure:
```
src/main/java/com/devnatalia/
├── api/
│   ├── controller/
│   ├── service/
│   ├── repository/
│   ├── model/
│   └── Application.java
```

## Testing

The project includes testing frameworks for both unit and integration tests. Place your test classes in the src/test directory.

## Version Information

- Project Version: 0.0.1-SNAPSHOT
- Java Version: 21
- Spring Boot Version: 4.0.3
- Group ID: com.devnatalia
- Artifact ID: api

## License

This project is open source and available for use and modification.


## Support and Contributions

For issues, questions, or contributions, please visit the repository at:
https://github.com/nalugao/api-java-spring-h2-db
