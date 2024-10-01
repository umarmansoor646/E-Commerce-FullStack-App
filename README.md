
## SOFTWARE ENGINEERING CAPSTONE
Welcome to Software Engineering Capstone! This is an opportunity for students to develop full stack software engineering documentation and applications. They will execute documentation, unit testing, revision of software applications, and deploy software applications with scripts and containers on a cloud platform.

Sure! Here’s a template for a README file for your e-commerce application. You can customize it based on your specific project details.

---

# E-Commerce Application

## Overview

This e-commerce fullstack application is designed to provide a seamless shopping experience. It is built with Angular for the front-end and Java Spring Boot for the back-end. The application supports user registration, product browsing, shopping cart management, and order processing.

## Features

- **User Authentication**: Register and log in to manage your account.
- **Product Catalog**: Browse and search for products.
- **Shopping Cart**: Add items to your cart and view cart details.
- **Checkout**: Complete your purchase with various payment options.
- **Order History**: View past orders and track their status.

## Technologies Used

- **Front-End**: Angular
- **Back-End**: Java Spring Boot
- **Database**: MySQL
- **Other Tools**: Docker (for containerization), Maven (for build automation)
- **Deployment**: Google Cloud (Cloud Sql, Cloud Run)

## Installation

### Prerequisites

- Java 11 or later
- Node.js and npm
- Docker (optional, for containerization)

### Clone the Repository
### Set Up the Back-End

1. **Navigate to the back-end directory**:

    ```bash
    cd backend
    ```

2. **Install dependencies**:

    ```bash
    ./gradlew build
    ```

3. **Run the back-end application**:

    ```bash
    ./gradlew bootRun
    ```

### Set Up the Front-End

1. **Navigate to the front-end directory**:

    ```bash
    cd frontend
    ```

2. **Install dependencies**:

    ```bash
    npm install
    ```

3. **Run the front-end application**:

    ```bash
    ng serve
    ```

### Docker Setup (Optional)

1. **Build the Docker image**:

    ```bash
    docker build -t your-app-name .
    ```

2. **Run the Docker container**:

    ```bash
    docker run -p 8080:8080 app-name
    ```

## Usage

1. **Access the Application**: Open your browser and go to `http://localhost:4200` to view the front-end application. The back-end API will be available at `http://localhost:8080`.

2. **Create an Account**: Register a new account to start shopping.

3. **Browse Products**: Use the search functionality or browse through categories.

4. **Add to Cart**: Add items to your shopping cart and view the cart summary.

5. **Checkout**: Proceed to checkout and complete your purchase.

6. **Manage Your Account**: Update your profile and view your order history.


---
