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

---


## API Endpoints

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



