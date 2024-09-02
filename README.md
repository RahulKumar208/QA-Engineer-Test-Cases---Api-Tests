# Kantox QA Engineer Challenge

This repository contains solutions for both parts of the challenge: creating test cases for a cashier system and testing an API using Postman.

## Part 1: Test Case Creation

### Cashier System

For Part 1 of the challenge, I have designed test cases for a simple cashier system that adds products to a cart and calculates the total price. The system supports the following products and discount rules:

**Products and Prices:**

| Product Code | Name         | Price |
|--------------|--------------|-------|
| GR1          | Green Tea    | £3.11 |
| SR1          | Strawberries | £5.00 |
| CF1          | Coffee       | £11.23|

**Discount Rules:**
- **FreeRule**: Buy N items, get N free.
- **ReducedPriceRule**: Buy more than N items, pay a reduced price per item.
- **FractionPriceRule**: Buy more than N items, pay a percentage of the original price.

The test cases cover scenarios such as:
- Adding various products to the cart.
- Applying different discount rules.
- Calculating total prices based on these rules.

The test cases are included in the file `Cashier_System_Test_Cases.xsls`.

---

## Part 2: API Test

### API Endpoints

For Part 2, I have created a Postman collection to test the following API endpoints hosted on a JSON Server:

- **GET /posts**
- **GET /posts/{id}**
- **POST /posts**
- **PUT /posts/{id}**
- **DELETE /posts/{id}**
- **GET /comments**
- **GET /comments/{id}**
- **POST /comments**
- **PUT /comments/{id}**
- **DELETE /comments/{id}**
- **GET /profile**

### Setup and Running the API

1. **Install Dependencies**:
    ```sh
    npm install
    ```

2. **Start the JSON Server**:
    ```sh
    npm start
    ```
    The server will run on `http://localhost:3000`.

### Postman Collection

- The Postman collection containing tests for the above endpoints is saved as `collection.json`.
- You can import this file into Postman to run the tests.

**How to Import the Collection into Postman:**

1. Open Postman.
2. Click on "Import" in the top-left corner.
3. Select "Upload Files" and choose `collection.json`.
4. Click "Import".

The collection will now be available in Postman, and you can run the tests for the various API endpoints.

---

## Setup and Installation

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/RahulKumar208/QA-Engineer-Test-Cases-and-Api-Tests.git
    cd qa-tech-test
    ```

2. **Install Dependencies for API Testing**:
    ```sh
    cd Part\ 2
    npm install
    ```

3. **Start the JSON Server**:
    ```sh
    npm start
    ```

---

## Additional Notes

- Ensure that the JSON Server is running before importing and running the Postman collection.
- The test cases in Part 1 are provided as a Markdown file in the root directory. They include scenarios and expected outcomes.

Feel free to reach out if you have any questions or need further clarification.
