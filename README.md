Ecommerce Microservices - Combined Repository
This repository contains all microservices required for a fully functional Ecommerce Platform.
Each microservice is maintained inside its own folder for better modularity and separation of concerns.

📁 Repository Structure

Ecommerce-Microservice/
├── ApiGateway/
├── EmailNotificationService/
├── Eureka/
├── OrderService/
├── PaymentService/
├── ProductService/
├── UserSelfService/
└── README.md
📚 Microservices Overview
1. ApiGateway
Repo Link: https://github.com/Ridhim-RR/ApiGateway

Acts as a single entry point into the system.

Routes requests to the appropriate microservices.

Provides features like load balancing, routing, and security.

2. EmailNotificationService
Repo Link: https://github.com/Ridhim-RR/Email-Notification-Service

Responsible for sending email notifications such as order confirmations, payment updates, etc.

Listens to events from other services and triggers emails accordingly.

3. Eureka (Service Registry)
Repo Link: https://github.com/Ridhim-RR/EurekaServer

Handles service discovery.

Registers all microservices dynamically so they can find and communicate with each other without hard-coding network locations.

4. OrderService
Repo Link: https://github.com/Ridhim-RR/Ecommerce-Order-Service

Manages everything related to customer orders.

Handles order placement, order tracking, and maintaining order history.

5. PaymentService
Repo Link: https://github.com/Ridhim-RR/Ecommerce-Payment-Service

Manages payment processing.

Integrates with external payment gateways to handle payments securely.

6. ProductService
Repo Link: https://github.com/Ridhim-RR/Ecommerce-Website

Manages product catalog, product details, inventory, etc.

Provides APIs for searching, viewing, and managing products.

7. UserSelfService
Repo Link: https://github.com/Ridhim-RR/UserSelfService

Handles user authentication, registration, profile management, and user-specific actions.

📦 How This Works Together
Eureka: All services register themselves here at startup.

ApiGateway: All incoming client requests go through the Gateway, which routes them to the correct service.

UserSelfService: Manages users and login/authentication.

ProductService: Manages products available for users to browse and purchase.

OrderService: Handles order creation when a user places an order.

PaymentService: Processes the payment for the order.

EmailNotificationService: Sends confirmation emails after orders/payments.

🚀 Getting Started
Start Eureka Server first.

Start ApiGateway.

Start UserSelfService, ProductService, OrderService, PaymentService, and EmailNotificationService.

Use the ApiGateway endpoints to access all services.

🛠 Tech Stack
Java 17+

Spring Boot

Spring Cloud (for Eureka, Config, etc.)

Spring Security (for authentication and authorization)

Kafka (optional, for async communication between services like Email Notification)

MySQL 

Maven

📖 Notes
Each subproject contains its own README.md for specific setup and running instructions.

This combined monorepo setup helps to easily manage and deploy all services together.


