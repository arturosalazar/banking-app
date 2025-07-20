# Digital Banking System with Real-Time Notifications and Fraud Detection

A backend project built with **Spring Boot**, demonstrating core software engineering skills including **Object-Oriented Design**.

This project simulates a realistic digital banking system that supports user account management, transaction processing (deposit, withdrawal, transfer), fraud detection, and real-time notifications — all backed by a clean, modular, and testable architecture.

---

## Project Goals

- Build a **realistic, modular, and scalable** banking backend.
- Demonstrate core **Java and Spring Boot** backend development skills.
- Apply **Object-Oriented Programming** (OOP) principles effectively.
- Showcase **clean architecture**, **security**, and **testing best practices**.
- Incorporate **event-driven design**.

---

## 🧱 Planned Architecture

```plaintext
banking-app/
├── controller/      --> REST APIs for account and transaction operations
├── service/         --> Business logic
├── domain/          --> Core domain models: Account, Transaction, etc.
├── repository/      --> Spring Data JPA repositories for persistence
├── dto/             --> Data Transfer Objects for input/output
├── security/        --> Authentication, authorization, role management
├── events/          --> Event publishing and handling
├── config/          --> Centralized configuration
└── resources/
    └── application.properties  --> App configuration
```

## Key OOP Concepts Demonstrated
Concept	Example
Abstraction	Abstract Transaction base class
Inheritance	DepositTransaction, WithdrawalTransaction extend Transaction
Encapsulation	Account fields are private with public accessors
Polymorphism	TransactionProcessor handles any subclass of Transaction

## Core Features
🧑‍💼 User Account Management
Create and manage user accounts

Support for multiple account types (e.g., checking, savings)

Balance tracking and validation

💰 Transaction Processing
Deposit, withdrawal, and internal transfers

Encapsulated transaction business logic

OOP-modeled transaction types

🛡️ Fraud Detection Module
Plug-and-play strategy pattern (e.g., high-value, velocity checks)

Modular design for future microservice separation

🔔 Real-Time Notifications
Alerts via Spring Events or Kafka

Simulated email/SMS delivery (console logs for now)

Listener-based decoupled notification system

🔐 Security
Spring Security with login, roles (e.g., USER, ADMIN)

JWT-based authentication (optional)

Endpoint access control

🧪 Testing
Unit and integration testing using JUnit 5 and Mockito

Test coverage for services, controllers, and fraud detection logic

🌐 API Design
Clean, RESTful endpoints

Swagger/OpenAPI documentation for testing and discovery

## 🛢️ Tech Stack
Layer	Technology
Language	Java 21
Framework	Spring Boot
Database	PostgreSQL
ORM	Spring Data JPA
Security	Spring Security
Messaging	Spring Events or Kafka (TBD)
Testing	JUnit, Mockito
Documentation	Swagger/OpenAPI
Dev Tools	Lombok, Spring DevTools
Optional Tools	Docker, GitHub Actions, Render/Railway