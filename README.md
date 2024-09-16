# Account Management Service with Docker Integration

This project is an Account Management Service built using Java Spring Boot. It demonstrates a microservice architecture that manages customer accounts, providing features such as adding, withdrawing, and deleting money from accounts. The service is containerized using Docker and uses MySQL as the database backend, managed through Docker Compose.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

What things you need to install the software and how to install them.

- Docker
- Docker Compose

### Installing

A step-by-step series of examples that tell you how to get a development environment running.

#### 1. Create a project folder and clone the Account Management service
```bash
mkdir dockerhub-assignment && cd dockerhub-assignment
git clone https://github.com/itshivam242/account-management-service-dockerhub.git ./
```
#### 2. Start the Docker Containers
Once the repository is cloned, use Docker Compose to start the service. This will pull the necessary Docker images and start the containers for the MySQL database and the Account Management Service.
```bash
docker-compose up
```
#### 3. Verify the Application

Once Docker Compose has finished setting up, you can verify the application by accessing the Account Management Service at:
```bash
http://localhost:8091/accounts
````
Check API endpoints below in this file to check application on postman.
#### 4. Stop the Application
Once the repository is cloned, use Docker Compose to start the service. This will pull the necessary Docker images and start the containers for the MySQL database and the Account Management Service.
```bash
docker-compose down
```
## Usage

The following API endpoints are available for managing accounts:

1. **Create a new account**
    - **HTTP Method:** POST
    - **Endpoint:** `/accounts`

2. **Add money to an account**
    - **HTTP Method:** PUT
    - **Endpoint:** `/accounts/add-money/{accountId}`

3. **Withdraw money from an account**
    - **HTTP Method:** PUT
    - **Endpoint:** `/accounts/withdraw-money/{accountId}`

4. **Get account details by account ID**
    - **HTTP Method:** GET
    - **Endpoint:** `/accounts/{accountId}`

5. **Delete an account**
    - **HTTP Method:** DELETE
    - **Endpoint:** `/accounts/{accountId}`

6. **Delete account by customer ID**
    - **HTTP Method:** DELETE
    - **Endpoint:** `/accounts/customers/{customerId}`



