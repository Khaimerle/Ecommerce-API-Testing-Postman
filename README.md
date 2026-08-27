# Ecommerce-API-Testing-Postman

## 📌 Project Overview

This project demonstrates API testing of an e-commerce REST API using **Postman**. The test suite covers product, user, authentication, and cart endpoints through positive and negative test scenarios.

The project focuses on validating API responses, HTTP status codes, response data, authentication, CRUD operations, and business logic.

## 🛠️ Tools & Technologies

- **Postman**
- **JavaScript** — API test scripts and assertions
- **REST API**
- **DummyJSON** — Practice API
- **GitHub** — Project documentation and version control

## 🧪 Test Coverage

### Products

- Get all products
- Get a specific product
- Get an invalid product
- Search products
- Filter products by category
- Add a product
- Update a product
- Delete a product

### Authentication

- Login with valid credentials
- Login with invalid credentials
- Get authenticated user
- Test invalid/expired token
- Test missing authentication token

### Users

- Get all users
- Get a specific user
- Get an invalid user
- Search users

### Carts

- Get all carts
- Get a specific cart
- Get carts by user
- Get an invalid cart
- Add a product to cart
- Update a cart
- Validate cart total using business logic

## 🔍 Testing Techniques

- Positive testing
- Negative testing
- Status code validation
- JSON response validation
- Response field validation
- Array validation
- Query parameter testing
- Path parameter testing
- Authentication testing
- CRUD testing
- Business logic validation
- Automated assertions
- Collection Runner execution

## 🔐 Authentication Testing

The authentication tests cover both successful and unsuccessful authentication scenarios.

An access token is automatically extracted from the login response and stored as a Postman environment variable.

```javascript
const data = pm.response.json();

pm.environment.set("accessToken", data.accessToken);
