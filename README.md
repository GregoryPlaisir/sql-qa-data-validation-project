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

## Skills Demonstrated

### SQL Skills

- SELECT
- WHERE
- ORDER BY
- DISTINCT
- LIKE
- BETWEEN
- COUNT
- SUM
- AVG
- MIN / MAX
- GROUP BY
- HAVING
- JOINs

### QA Skills

- Backend Data Validation
- Test Data Review
- Defect Identification
- Business Rule Validation
- Requirements Verification
- Data Integrity Testing
- UAT Support

---

## Project Structure

```text
sql-qa-data-validation-project/

database/

queries/

documentation/

screenshots/

findings/
