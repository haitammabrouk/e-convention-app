# Internship Agreement Digitalization Platform

## Project Overview

This web application streamlines and automates the manual internship agreement signing process previously used by the school. It replaces time-consuming manual steps — downloading forms, filling them out, physically signing, and submitting documents — with a fully digital, efficient workflow.improving overall user experience.

## Technology Stack

- Backend: Spring Boot (Java 17)  
- Frontend: Angular 16.2.8  
- Database: PostgreSQL  

## Prerequisites

- Docker installed on your system  
- Java 17 or higher  
- Node.js (recommended recent stable version)  
- Angular CLI (version 16.2.8)  
- PostgreSQL container exposed on port 5432
- Minio container exposed on port 9000

### 1. Clone the repository
```bash
https://github.com/haitammabrouk/e-convention-app.git
cd e-convention-app
```

### 2. Configure PostgreSQL
Run up a PostgreSQL container and update the database connection details in the backend configuration file located at:

```
src/main/resources/application.properties
```

Provide your database URL, username, and password.

### 3. Build and run the backend

```bash
cd e-convention-backend
./mvnw clean install
./mvnw spring-boot:run
```

This will start the backend server at http://localhost:8080 by default.

### 4. Build and run the frontend

```bash
cd e-convention-frontend
npm install
ng serve
```

The frontend will be available at http://localhost:4200.
