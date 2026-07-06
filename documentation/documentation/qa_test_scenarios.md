# QA Test Scenarios

## Overview

This document outlines the QA validation scenarios for the SQL QA Data Validation Project.

The goal is to demonstrate how a QA Engineer uses SQL to validate data integrity, verify business rules, and identify backend data defects.

---

## Test Coverage Summary

| Scenario ID | Scenario | Requirement | Validation Type |
|---|---|---|---|
| TS-001 | Customer Email Uniqueness | Customer emails must be unique | Data Validation |
| TS-002 | Required Customer Fields | Customer first name, last name, and email are required | Data Completeness |
| TS-003 | Product Pricing Validation | Product prices must be greater than $0 | Business Rule Validation |
| TS-004 | Customer-to-Order Relationship | Every order must belong to a valid customer | Relationship Validation |
| TS-005 | Product-to-Order Relationship | Every order must reference a valid product | Relationship Validation |
| TS-006 | Sales Totals Validation | Order totals should accurately reflect sales activity | Aggregate Validation |

---

## Detailed Test Scenarios

### TS-001: Customer Email Uniqueness

**Requirement:**  
Each customer must have a unique email address.

**Validation Approach:**  
Use SQL to group customer records by email address and identify duplicates.

**Expected Result:**  
No duplicate email addresses should exist.

**Related Query File:**  
`queries/data_validation_queries.sql`

---

### TS-002: Required Customer Fields

**Requirement:**  
Customer records must include first name, last name, and email address.

**Validation Approach:**  
Use SQL to identify null or blank values in required customer fields.

**Expected Result:**  
All required customer fields should contain valid data.

**Related Query File:**  
`queries/data_validation_queries.sql`

---

### TS-003: Product Pricing Validation

**Requirement:**  
All products must have a price greater than $0.

**Validation Approach:**  
Use SQL to identify products with missing, zero, or negative pricing.

**Expected Result:**  
All products should have valid pricing greater than $0.

**Related Query File:**  
`queries/data_validation_queries.sql`

---

### TS-004: Customer-to-Order Relationship

**Requirement:**  
Every order must be associated with a valid customer.

**Validation Approach:**  
Use JOIN queries to identify orders that do not match an existing customer record.

**Expected Result:**  
Every order should reference a valid customer.

**Related Query File:**  
`queries/join_queries.sql`

---

### TS-005: Product-to-Order Relationship

**Requirement:**  
Every order must reference a valid product.

**Validation Approach:**  
Use JOIN queries to identify orders that do not match an existing product record.

**Expected Result:**  
Every order should reference a valid product.

**Related Query File:**  
`queries/join_queries.sql`

---

### TS-006: Sales Totals Validation

**Requirement:**  
Sales totals should accurately reflect order activity.

**Validation Approach:**  
Use aggregate SQL functions to calculate total sales, average order value, and sales by date.

**Expected Result:**  
Sales totals should match expected reporting values.

**Related Query File:**  
`queries/aggregate_queries.sql`

---

## QA Notes

These scenarios are designed to reflect common backend validation tasks performed by QA Analysts, UAT Analysts, QA Engineers, and Application Support teams.

Each scenario connects a business requirement to a SQL validation approach, helping demonstrate both technical skill and QA thinking.
