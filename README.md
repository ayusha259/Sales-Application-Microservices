# Sales Application Microservices

## Architecture Overview

The backend for the retail shopping application is built using Node.js and follows a microservice-based architecture. This design comprises three key services, each focusing on distinct functionalities:

### 1. Customer Management Service
- **Functions**: Handles customer registration, login processes, and profile management.
- **Objective**: To deliver a streamlined user experience by managing all customer interactions.

### 2. Shopping Cart Service
- **Functions**: Manages shopping cart operations, processes orders, and tracks order statuses.
- **Objective**: To provide an efficient and intuitive shopping experience for users.

### 3. Product Management Service
- **Functions**: Oversees product listings, detailed product information, and inventory control.
- **Objective**: To ensure accurate representation and management of product data.

## System Components

### Message Broker
- **Purpose**: Ensures effective communication between microservices.
- **Benefits**: Maintains service autonomy and minimizes the risk of widespread system failures.

### Supporting Components
- **Database**: Stores essential user and product data.
- **API Gateway**: Manages incoming requests from the frontend interface.
- **Load Balancer**: Distributes traffic to maintain performance under high load conditions.

## Database Strategy

### Database per Service
- **Description**: Each microservice operates with its own dedicated database.
- **Benefits**: Enhances scalability and load distribution.
- **Challenges**: Managing data consistency across multiple databases.

## Advantages and Disadvantages of Microservices

### Advantages
- **Modular Design**: Facilitates independent development and deployment.
- **Scalability**: Enables scaling of individual services based on demand.
- **Fault Isolation**: Limits impact of failures to specific services, enhancing resilience.

### Disadvantages
- **Complexity**: Increased management and operational complexity.
- **Data Management**: Potential difficulties in maintaining data consistency.
- **Communication Latency**: Possible delays in interactions between services.

## Important Notes
- **Configuration**: Ensure to update the MongoDB and RabbitMQ connection strings in the `.env.dev` file before initiating the services.

For further details on each service and component, please refer to the sections above.

---