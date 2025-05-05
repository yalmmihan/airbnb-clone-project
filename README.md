# Airbnb Clone Project

The Airbnb Clone Project is a comprehensive, real-world application designed to simulate the development of a robust booking platform like Airbnb. It focuses on backend systems, database design, API development, and application security.

---

## Project Goals

- Learn how to build a scalable backend system.
- Improve understanding of team collaboration using GitHub.
- Implement modern security and CI/CD practices.
- Design a structured and efficient database.
- Use Django, MySQL, GraphQL and Docker in a unified full-stack project.

---

## Team Roles

- *Backend Developer*: Implements the application logic, API endpoints, and backend integration.
- *Frontend Developer*: Designs the user interface and connects it with backend APIs.
- *Database Administrator (DBA)*: Designs and manages the database schema, ensures data integrity and performance.
- *DevOps Engineer*: Sets up CI/CD pipelines, manages server environments, and automates deployment.
- *Project Manager*: Oversees the progress, distributes tasks, and ensures milestones are met.

---

## Technology Stack

- *Django*: A Python web framework used for building robust and scalable backend systems and RESTful APIs.
- *MySQL*: A relational database used to store and manage user, property, and booking data.
- *GraphQL*: A query language used to fetch data efficiently and flexibly from the backend.
- *Docker*: Containerization tool to package the application for consistent deployment.
- *GitHub Actions*: Automation tool used to implement CI/CD pipelines for testing and deployment.

---

## Database Design

### *Entities & Key Fields:*

- *User*
  - id
  - name
  - email
  - password
  - role (host/guest)

- *Property*
  - id
  - title
  - description
  - location
  - user_id (owner)

- *Booking*
  - id
  - user_id (guest)
  - property_id
  - start_date
  - end_date

- *Review*
  - id
  - user_id
  - property_id
  - rating
  - comment

- *Payment*
  - id
  - booking_id
  - amount
  - payment_method
  - status

### *Relationships:*
- One *User* can have many *Properties*.
- One *Property* can have many *Bookings* and *Reviews*.
- One *Booking* has one *Payment*.

---

## Feature Breakdown

- *User Management*: Allows registration, login, profile editing, and role management (host or guest).
- *Property Management*: Hosts can add, update, and delete listings including photos and descriptions.
- *Booking System*: Guests can search for properties, view availability, and make bookings.
- *Review System*: Guests can leave reviews after their stay, with ratings and comments.
- *Payment System*: Secure payments linked to bookings, with tracking of status and method.

---

## API Security

- *Authentication*: Users must login with secure tokens (JWT) to access private routes.
- *Authorization*: Only hosts can manage properties, and only guests can book.
- *Rate Limiting*: Prevents abuse by limiting the number of API requests per user.
- *Input Validation*: Prevents malicious data from entering the system.
- *Data Encryption*: Sensitive data like passwords are encrypted using industry best practices.

---

## CI/CD Pipeline

- *Continuous Integration (CI)*: Automatically runs tests whenever code is pushed to GitHub.
- *Continuous Deployment (CD)*: Automatically deploys to staging or production when tests pass.
- *Tools Used*:
  - *GitHub Actions*: For automation of testing and deployment.
  - *Docker*: For containerization and deployment consistency.
  - *Heroku/AWS*: (optional) for hosting the application.

---
