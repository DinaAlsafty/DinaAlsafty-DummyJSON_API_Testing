# API Testing Project – DummyJSON

## 📌 Project Overview

This project demonstrates practical **API testing using Postman** on the DummyJSON REST API.

The project covers functional, positive, and negative API testing across **Authentication, Products, Users, and Carts**.

Test scenarios and test cases were designed, executed, and validated using **Postman JavaScript assertions**, with execution results documented in QA test reports.

---

## 🎯 Project Objectives

The main objectives of this project were to:

* Validate API functionality and response behavior.
* Verify HTTP status codes and response structures.
* Perform positive and negative testing.
* Validate authentication and authorization behavior.
* Test CRUD operations.
* Validate search, filtering, and pagination functionality.
* Validate response data using JavaScript assertions.
* Execute the complete Postman collection using Collection Runner.
* Document test execution results and test outcomes.

---

## 🛠️ Tools & Technologies

* **Postman**
* **JavaScript** – Postman test scripts
* **REST API**
* **JSON**
* **Microsoft Excel**
* **GitHub**

---

## 🧩 Modules Tested

### 1. Authentication API

Tested:

* User login
* Login with invalid credentials
* Access token validation
* Refresh token validation
* Retrieving authenticated user with a valid access token
* Authentication without an access token
* Authentication using an invalid access token

### 2. Products API

Tested:

* Retrieve all products
* Retrieve product by ID
* Invalid product ID
* Product search
* Search with no matching results
* Product categories
* Invalid category
* Limit and pagination
* Selected fields
* Sorting
* Product creation
* Product update using PUT
* Partial update using PATCH
* Product deletion

### 3. Users API

Tested:

* Retrieve all users
* Retrieve user by ID
* Invalid user ID
* User search
* Search with no matching results
* Limit and pagination
* Selected fields
* Sorting
* User filtering
* Invalid filter scenarios
* User creation
* User update using PUT
* Partial update using PATCH
* User deletion

### 4. Carts API

Tested:

* Retrieve all carts
* Retrieve cart by ID
* Invalid cart ID
* Retrieve carts by user ID
* Invalid user ID
* Limit and pagination
* Selected fields
* Sorting

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
* CRUD Testing
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

> A 100% pass rate reflects the results of the defined and executed test cases. It does not imply that the API is completely free of defects.

---

## 📁 Project Artifacts

### Postman

* `Postman_collection.json` – Postman API testing collection containing requests and JavaScript assertions.
* `Postman Test Run Results.json` – Exported Postman collection execution results.

### Test Documentation

* `Test_Scenarios.xlsx` – Designed API test scenarios.
* `Testcases.xlsx` – Detailed API test cases.
* `TestCases_execution.xlsx` – Test case execution results.
* `Execution & Summary Report.xlsx` – Test execution and summary reporting.

---

## ▶️ How to Run the Tests

1. Download or clone this repository.
2. Open **Postman**.
3. Import `Postman_collection.json`.
4. Configure the required environment variables if applicable.
5. Select the appropriate environment.
6. Run the collection using **Collection Runner**.
7. Review the requests and JavaScript assertions.
8. Review the execution results.

---

## 📌 Project Outcome

This project demonstrates practical experience in **REST API testing using Postman**, including:

* API test scenario and test case design
* Positive and negative testing
* Authentication and authorization testing
* CRUD operations
* HTTP status code validation
* Response structure validation
* JSON response validation
* Search and filtering testing
* Pagination testing
* JavaScript assertions
* Collection Runner execution
* Test execution reporting
* QA documentation

The project demonstrates the application of a structured testing workflow:

**Test Scenarios → Test Cases → Test Execution → Validation → Reporting**

---
