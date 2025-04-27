# Eureka Server

A Eureka Server for service discovery in a microservices architecture.  
Enables dynamic registration and lookup of Spring Boot microservices to simplify inter-service communication.

## Features

- Acts as a central registry for all microservices
- Supports client-side load balancing via Eureka clients
- Automatically updates registry as services come online or go offline

## How It Works

- Microservices register themselves with the Eureka Server
- Other services can discover these registered instances using service IDs
- Works seamlessly with Spring Cloud and Netflix Eureka

## Setup

1. Clone the repository
2. Run the Eureka server on default port (e.g. `8091`)
3. Configure your other services to register with the Eureka server:
