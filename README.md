# Smart-Skill-Based-Task-Marketplace-AI-Assisted-
An industry-grade, event-driven microservices platform that connects clients with skilled freelancers through secure authentication, task management, bidding workflows, and real-time notifications.  This project is being actively developed using modern backend, frontend, and DevOps technologies following real-world software engineering practices.

#Overview

The **Smart Skill-Based Task Marketplace** allows:
- Clients to post tasks with required skills and budget
- Freelancers to browse tasks and submit bids
- Secure task assignment, tracking, and reviews
- Event-driven communication between services
- Scalable and maintainable microservices architecture

The system is designed to simulate how real-world freelance and talent marketplaces work, focusing on **scalability, security, and clean design**.

## 🏗️ System Architecture (High Level)
Frontend (React + Tailwind)
|
v
API Gateway (Spring Cloud Gateway)
|

| | | | | |
Auth Profile Task Bid Review Notification
Service Service Service Service Service Service
|
Kafka (Event Bus)
|
MySQL Database


# Repository Structure
smart-skill-marketplace/
├── backend/
│   ├── api-gateway/
│   ├── auth-service/
│   ├── task-service/
│   ├── bid-service/
│   └── docker-compose.yml
├── frontend/
│   └── skill-marketplace-ui/
├── design/
│   ├── HLD.md
│   ├── LLD.md
│   └── events.md
└── README.md


# Additional Information

---

## 🧩 Microservices Breakdown

| Service Name | Responsibility |
|-------------|----------------|
| API Gateway | Central entry point, routing, security |
| Auth Service | Signup, login, JWT authentication |
| Profile Service | User skills, experience, portfolio |
| Task Service | Task creation and management |
| Bid Service | Freelancer proposals and bidding |
| Matching Service | Skill-based matching (rule-based currently) |
| Review Service | Ratings and feedback |
| Notification Service | Email / real-time notifications |
| Service Registry | Eureka discovery server |
| Config Server | Centralized configuration |

---

## 🔐 Security Design

- Implemented **Spring Security with JWT**
- Role-Based Access Control (RBAC):
  - CLIENT
  - FREELANCER
  - ADMIN
- Password encryption using **BCrypt**
- Token validation handled via API Gateway

---

## 🔁 Event-Driven Architecture (Kafka)

Kafka is used to decouple services and enable asynchronous processing.

### Example Events:
- `TASK_CREATED`
- `BID_SUBMITTED`
- `TASK_ASSIGNED`
- `TASK_COMPLETED`
- `REVIEW_ADDED`

This ensures:
- Loose coupling between services
- Better scalability
- Fault tolerance

---

## 🛠️ Tech Stack

### Backend
- Java 17
- Spring Boot
- Spring Security
- Spring Cloud (Gateway, Eureka, Config)
- Spring Data JPA
- Apache Kafka
- MySQL

### Frontend
- React
- Tailwind CSS
- React Router

### DevOps & Tools
- Docker & Docker Compose
- Jenkins (CI/CD – in progress)
- Git & GitHub
- Postman
- Eclipse IDEA

---

## 🧪 How to Run (Local Setup)

> Prerequisites:
- Java 17
- Docker & Docker Compose
- Node.js (LTS)
- Maven

### Start Infrastructure into bash
docker-compose up -d

# Project Implementation Summary
1. Designed an industry-grade microservices architecture using Spring Boot and Spring Cloud, separating core domains such as authentication, user profiles, task management, bidding,       reviews, and notifications.
2. Implemented secure authentication and authorisation using Spring Security with JWT, enabling role-based access control for CLIENT, FREELANCER, and ADMIN users.
3. Developed RESTful APIs for task posting, bid submission, task assignment, and review management using Spring Data JPA with MySQL for transactional consistency.
4. Integrated Apache Kafka to implement an event-driven architecture, allowing asynchronous communication between services for task creation, bid submission, task assignment, and      notification workflows.
5. Configured API Gateway and Eureka Service Discovery to provide centralised routing, load balancing, and dynamic service registration.
6. Containerised backend services, Kafka, and MySQL using Docker and Docker Compose to ensure consistent local and production-like environments.
7. Built a React + Tailwind CSS frontend with role-based dashboards, enabling users to interact with backend services through a clean and intuitive UI.
8. Set up CI/CD pipelines using Jenkins to automate build, test, and Docker image creation processes.
9. Followed clean architecture principles, SOLID design, and proper documentation (HLD/LLD) to ensure scalability, maintainability, and ease of future enhancements.


## 🔮 Future Enhancements

- AI-based skill matching and ranking
- ElasticSearch for advanced task search
- Kubernetes deployment
- Payment & escrow simulation
- Monitoring with Prometheus and Grafana
- Fraud detection and reputation scoring

---


 ## Author
Aniket Singh
Java Backend Developer | Spring Boot | Microservices
Actively learning and building industry-grade backend systems.



