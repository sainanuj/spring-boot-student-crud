# Spring Boot Student CRUD API

REST API for student management built with Spring Boot 4.0.6, Java 21, and MySQL 9.7.

## Tech Stack
- **Java 21** - OpenJDK 21.0.10
- **Spring Boot 4.0.6** - Latest major version
- **Spring Data JPA** - Hibernate 7.2.12.Final
- **MySQL 9.7.0** - Running in Docker
- **Maven** - Dependency management
- **Lombok** - Boilerplate reduction

## Features
- ✅ Create, Read, Update, Delete students
- ✅ MySQL integration with HikariCP connection pool
- ✅ Auto DDL via Hibernate `ddl-auto=update`
- ✅ RESTful endpoints under `/api/students`
- ✅ DevTools for hot reload

## Prerequisites
1. JDK 21 installed
2. Docker + Docker Compose
3. Maven 3.9+ or use included `mvnw`

## Quick Start

### 1. Start MySQL with Docker
```bash
docker run --name mysql-db \
  -e MYSQL_ROOT_PASSWORD=yourpassword \
  -e MYSQL_DATABASE=studentdb \
  -p 3306:3306 \
  -d mysql:9.7.0