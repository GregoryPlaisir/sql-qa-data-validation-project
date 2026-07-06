# Validation Findings

## Overview

This document tracks data validation findings, business rule violations, and defects identified during SQL testing.

The purpose of this document is to demonstrate how SQL can be used to validate requirements, identify data quality issues, and communicate findings in a structured QA format.

---

## Findings Dashboard

| Finding ID | Description | Severity | Status |
|------------|-------------|----------|--------|
| F-001 | Duplicate Customer Email | Medium | Planned |
| F-002 | Missing Customer Email | High | Planned |
| F-003 | Invalid Product Price | Medium | Planned |
| F-004 | Order Without Customer | High | Planned |
| F-005 | Order Without Product | High | Planned |

---

## Finding Documentation Template

### Finding ID

F-XXX

### Related Test Scenario

TS-XXX

### Requirement

Document the business requirement being validated.

### Validation Query

Reference the SQL query used to identify the issue.

### Expected Result

Describe the expected system behavior.

### Actual Result

Document the observed result.

### Business Impact

Explain the impact to reporting, operations, users, or data integrity.

### Severity

- Low
- Medium
- High

### Status

- Open
- Closed
- Investigating

### Evidence

Link screenshots or query results.

---

## Future Findings

As validation queries are executed, planned findings will be replaced with actual defects, validation results, screenshots, and supporting evidence.

Each finding will be traceable to:

- A Test Scenario
- A Validation Query
- Supporting Evidence
- Business Impact Assessment
