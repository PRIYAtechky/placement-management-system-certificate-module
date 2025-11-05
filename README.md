# placement-management-system-certificate-module 🎓

This project is a **Certificate Management Module** that is part of the **Placement Management System**.  
It enables efficient handling of student certificates with **CRUD operations** using **Spring Boot**, **PostgreSQL**, and **Postman** for API testing.


## Features

- Add, view, update, and delete certificates  
- RESTful API for easy integration  
- Layered architecture (Controller, Service, Repository)  
- PostgreSQL database connectivity  
- Secure configuration with Spring Security  
- Tested and verified using Postman  

## Tech Stack

<p align="left">
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Spring%20Data%20JPA-0078D4?style=for-the-badge&logo=spring&logoColor=white" alt="Spring Data JPA" />
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" alt="Postman" />
  <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white" alt="Spring Security" />
  <img src="https://img.shields.io/badge/Java-F89820?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
</p>


| Component | Technology |
|------------|-------------|
| Backend | Spring Boot |
| Database | PostgreSQL |
| ORM | Spring Data JPA |
| API Testing | Postman |
| Security | Spring Security |
| Language | Java |

## API Endpoints

<p align="left">
  <img src="https://img.shields.io/badge/POST-0078D4?style=for-the-badge&logo=postman&logoColor=white" alt="POST" />
  <img src="https://img.shields.io/badge/GET-28A745?style=for-the-badge&logo=postman&logoColor=white" alt="GET" />
  <img src="https://img.shields.io/badge/PUT-FFC107?style=for-the-badge&logo=postman&logoColor=white" alt="PUT" />
  <img src="https://img.shields.io/badge/DELETE-DC3545?style=for-the-badge&logo=postman&logoColor=white" alt="DELETE" />
</p>


> These endpoints support full CRUD (Create, Read, Update, Delete) operations for managing certificate data.

| Method | Endpoint | Description |
|--------|-----------|-------------|
| **POST** | `/certificates` | Add a new certificate |
| **GET** | `/certificates` | Fetch all certificates |
| **GET** | `/certificates/{id}` | Fetch certificate by ID |
| **PUT** | `/certificates/{id}` | Update existing certificate |
| **DELETE** | `/certificates/{id}` | Delete certificate by ID |

## Example JSON (Postman Body)

```json
{
  "name": "AWS Certified Cloud Practitioner",
  "issuer": "Amazon Web Services",
  "issueDate": "2025-01-15",
  "expiryDate": "2028-01-15"
}
```
✅ Use POST → http://localhost:8083/certificates to add new certificates.
✅ Use PUT → http://localhost:8083/certificates/{id} to update.

## How It Works
1. Spring Boot connects to **PostgreSQL** via **Spring Data JPA**.  
2. The REST controller handles CRUD operations for `Certificate` entities.  
3. You can test all endpoints easily using **Postman**.  

**DI need to be added :**

JDBC API

Spring Data JPA

PostgreSQL Driver

Rest Repositories

Spring web

## How to Run

### 1.Clone the repository

```bash
git clone https://github.com/PRIYAtechky/PLACEMENT-MANAGEMENT-SYSTEM_certificate-module.git
cd PLACEMENT-MANAGEMENT-SYSTEM_certificate-module
```

### 2.Open the project

Import the project into Spring Tool Suite (STS) or IntelliJ IDEA as a Maven Project.

### 3.Configure the Database

Open pgAdmin or PostgreSQL CLI and create a database:

```mysql
CREATE DATABASE certificate_db;
```

Update your credentials in application.properties:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/certificate_db
spring.datasource.username=postgres
spring.datasource.password=postgres
```

### 4.Build and Run the Application

```bash
mvn spring-boot:run
```
or simply click Run → Run As → Spring Boot App in your IDE.

### 5.Access the Application

Base URL: ``` http://localhost:8083/certificate```

Test API endpoints using Postman for:

```POST``` → Add Certificate

```GET``` → View Certificates

```PUT``` → Update Certificate

```DELETE``` → Remove Certificate


