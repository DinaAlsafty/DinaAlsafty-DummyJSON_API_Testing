# API Testing Project – DummyJSON

## 📌 Project Overview

This project demonstrates practical **API testing using Postman** on the [DummyJSON REST API].

The project covers functional, positive, and negative API testing across multiple modules, with test cases designed, executed, and validated using **Postman JavaScript assertions**.

The testing process includes test scenario design, test case creation, test execution, response validation, defect analysis, and test reporting.

---

## 🎯 Project Objectives

The main objectives of this project were to:

* Validate API functionality and response behavior.
* Verify HTTP status codes and response structures.
* Perform positive and negative testing.
* Validate authentication and authorization behavior.
* Test search, filtering, and pagination functionality.
* Validate response data using JavaScript assertions.
* Execute the complete Postman collection using Collection Runner.
* Document test execution results and defects.

---

## 🛠️ Tools & Technologies

* **Postman**
* **JavaScript** – Postman test scripts
* **REST API**
* **JSON**
* **GitHub**
* **Excel** – Test documentation and reporting

---

## 🧩 Modules Tested

### 1. Authentication

Tested authentication-related API functionality, including:

* User login
* Access token validation
* Refresh token validation
* Authentication without an access token
* Invalid authentication scenarios

### 2. Products

Tested:

* Retrieve all products
* Search products
* Retrieve product by ID
* Invalid product ID
* Product creation
* Product update
* Product deletion
* Pagination
* Product response validation

### 3. Users

Tested:

* Retrieve all users
* Retrieve user by ID
* Invalid user ID
* Search users
* Invalid search keyword
* Limit and pagination
* Select specific user fields
* User filtering
* Invalid filter scenarios

### 4. Carts

Tested:

* Retrieve all carts
* Retrieve cart by ID
* Invalid cart ID
* Pagination
* Cart response validation

---

## 🧪 Testing Types

The project includes:

* Positive Testing
* Negative Testing
* Functional Testing
* API Response Validation
* Status Code Validation
* Authentication Testing
* Authorization Testing
* Search Testing
* Filtering Testing
* Pagination Testing
* Response Data Validation

---

## 🔍 API Test Automation & Assertions

Postman JavaScript assertions were implemented to automatically validate API responses.

Assertions were used to verify:

* HTTP status codes
* Response structure
* Required properties
* Data types
* Returned arrays
* Number of returned records
* Pagination parameters
* Access and refresh tokens
* Search results
* Filter results
* Response data

### Example

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Users are returned successfully", function () {
    const response = pm.response.json();

    pm.expect(response.users).to.be.an("array");
});
```

---

## 📊 Test Execution Summary

The complete Postman collection was executed using **Postman Collection Runner**.

| Metric                   | Result |
| ------------------------ | -----: |
| Total Requests           |     62 |
| Total Assertions / Tests |    144 |
| Passed                   |    144 |
| Failed                   |      0 |
| Blocked                  |      0 |
| Pass Rate                |   100% |
| Defects Identified       |      0 |

### Module Execution

| Module         | Requests |   Tests |  Passed | Failed |
| -------------- | -------: | ------: | ------: | -----: |
| Products       |       22 |      50 |      50 |      0 |
| Authentication |       11 |      24 |      24 |      0 |
| Users          |       19 |      45 |      45 |      0 |
| Carts          |       10 |      25 |      25 |      0 |
| **Total**      |   **62** | **144** | **144** |  **0** |

---

## 🐞 Defect Summary

No defects were identified during the executed test cycle.

All executed test assertions passed successfully.

> Note: A 100% pass rate reflects the results of the defined and executed test cases. It does not imply that the API is completely free of defects.

---

## 📁 Project Structure

```text
API-Testing-Project/
│
├── Postman/
│   └── DummyJSON API Testing.postman_collection.json
│
├── Test Documentation/
│   ├── Test Scenarios.xlsx
│   ├── Test Cases.xlsx
│   ├── Test Execution Report.xlsx
│   └── Test Summary Report.xlsx
│
├── Evidence/
│
└── README.md
```

---

## ▶️ How to Run the Tests

1. Open **Postman**.
2. Import the project collection.
3. Configure the required environment variables.
4. Select the appropriate environment.
5. Open the imported collection.
6. Run the collection using **Collection Runner**.
7. Review the executed requests and assertions.
8. Review the test execution results.

---

## 📄 Project Artifacts

The project includes:

* Postman Collection
* Test Scenarios
* Test Cases
* Test Execution Report
* Test Summary Report
* Execution Evidence

These artifacts demonstrate the complete testing workflow from **test design → execution → validation → reporting**.

---

## 📌 Project Outcome

This project demonstrates practical experience in **API testing using Postman**, including:

* API test case design
* Positive and negative testing
* Authentication and authorization testing
* HTTP status code validation
* Response structure validation
* Search and filtering testing
* Pagination testing
* JSON response validation
* JavaScript assertions
* Collection Runner execution
* Test execution reporting
* Defect analysis and reporting

The project demonstrates the ability to apply a structured software testing process to REST APIs and document the results using professional QA artifacts.

