# API Gateway
This is the API Gateway service for an e-commerce platform built using a microservices architecture with Spring Boot and Spring Cloud. The API Gateway acts as a reverse proxy that routes requests to various backend services (like product service, order service, payment service, etc.), providing a single entry point for all client interactions.


## Overview

The API Gateway is implemented using Spring Cloud Gateway, which provides a simple, yet flexible way to route requests to different microservices. It handles:

- Routing requests to appropriate services based on the URL or other criteria
- Load balancing
- Authentication and authorization
- Rate limiting and request throttling
- Request and response transformations

The API Gateway serves as the entry point for all client interactions and abstracts the underlying microservices.

## Features

- **Dynamic routing:** Routes requests based on URL paths, HTTP methods, or headers to appropriate microservices.
- **Load balancing:** Distributes traffic evenly across multiple instances of the same service.
- **Security:** Supports JWT-based authentication and authorization.
- **Rate limiting:** Configurable to protect against high traffic spikes and ensure fair usage.
- **Circuit breaking:** Handles failures gracefully by providing fallback mechanisms.
- **Service discovery:** Integrates with Spring Cloud's Eureka server to discover microservices.

## Setup

### Prerequisites

Before you begin, ensure that you have the following installed:

- Java 21
- Maven

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/akram-idrissi/Borcell-API-Gateway.git
   cd Borcell-API-Gateway
   ```
2. mvn clean install
3. mvn spring-boot:run
4. open browser got to: http://localhost:8072
