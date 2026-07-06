# SQL QA Data Validation Project

## 🎯 Project Objective

This project demonstrates how SQL can be used in Quality Assurance testing to validate data integrity, verify business rules, identify defects, and support backend testing.

The project simulates an e-commerce application with customer, product, and order data. As the QA Engineer, the goal is to use SQL queries to confirm that the database records are accurate, complete, and aligned with expected business requirements.

---

## 🧩 Business Scenario

An online retail company stores customer, product, and order information in a relational database.

QA is responsible for validating that:

- Customer records are complete and accurate
- Product records contain valid pricing
- Orders are connected to valid customers
- Orders are connected to valid products
- Sales totals are calculated correctly
- Business rules are followed before release

---

## 🧪 QA Testing Scenarios

The following scenarios simulate common backend validation activities performed by Quality Assurance Engineers.

### Scenario 1: Validate Customer Email Uniqueness

**Requirement:**
Each customer must have a unique email address.

**Validation Goal:**
Identify duplicate customer email records.

---

### Scenario 2: Validate Customer Required Fields

**Requirement:**
All customers must have a first name, last name, and email address.

**Validation Goal:**
Identify incomplete customer records.

---

### Scenario 3: Validate Product Pricing

**Requirement:**
Products must have a valid price greater than $0.

**Validation Goal:**
Identify products with missing or invalid pricing.

---

### Scenario 4: Validate Customer-to-Order Relationships

**Requirement:**
Every order must belong to a valid customer.

**Validation Goal:**
Identify orphaned order records.

---

### Scenario 5: Validate Product-to-Order Relationships

**Requirement:**
Every order must reference a valid product.

**Validation Goal:**
Identify orders linked to invalid products.

---

### Scenario 6: Validate Sales Totals

**Requirement:**
Order amounts should accurately reflect sales activity.

**Validation Goal:**
Verify aggregate sales calculations using SQL.
---

---

## 🛠 Skills Demonstrated

### SQL Skills

- SELECT Statements
- Filtering with WHERE
- Sorting with ORDER BY
- DISTINCT Queries
- Wildcard Searches with LIKE
- Aggregate Functions (COUNT, SUM, AVG, MIN, MAX)
- GROUP BY
- HAVING
- INNER JOINs
- Data Validation Queries

### Quality Assurance Skills

- Backend Data Validation
- Requirements Verification
- Business Rule Validation
- Defect Identification
- Test Scenario Design
- Root Cause Analysis
- Data Integrity Testing
- UAT Support

### Tools & Technologies

- SQL
- MySQL
- Git
- GitHub
- VS Code
- Excel

### Professional Skills

- Analytical Thinking
- Problem Solving
- Stakeholder Communication
- Documentation
- Test Planning
- Defect Reporting

  ---

## 📸 Evidence & Findings

As this project progresses, screenshots, query results, validation findings, and defect examples will be documented below.

The goal is not only to demonstrate SQL knowledge, but also to showcase how SQL is used in Quality Assurance to validate requirements, identify defects, and verify data integrity.

### Planned Evidence

- Database Schema Screenshots
- SQL Query Screenshots
- Query Result Screenshots
- Data Validation Results
- Defect Examples
- Requirements Validation Examples
- Business Rule Validation Results

---

## 🐞 Sample Findings Format

### Finding #1: Duplicate Customer Email Detected

**Requirement:**
Each customer must have a unique email address.

**Expected Result:**
No duplicate email addresses should exist.

**Actual Result:**
Multiple customer records were found sharing the same email address.

**Impact:**
Duplicate communications and inaccurate customer reporting may occur.

**Status:**
Defect Identified

---

### Finding #2: Missing Customer Email

**Requirement:**
Customer email is a required field.

**Expected Result:**
All customer records contain a valid email address.

**Actual Result:**
One or more customer records were missing an email address.

**Impact:**
Customer notifications cannot be delivered.

**Status:**
Defect Identified

---

## 📂 Project Structure

sql-qa-data-validation-project/

database/
- create_tables.sql
- insert_data.sql

queries/
- basic_queries.sql
- aggregate_queries.sql
- data_validation_queries.sql
- join_queries.sql

documentation/
- qa_test_scenarios.md

screenshots/
- schema
- query-results
- findings

findings/
- validation-findings.md

README.md
