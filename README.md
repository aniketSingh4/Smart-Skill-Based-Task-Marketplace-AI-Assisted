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
