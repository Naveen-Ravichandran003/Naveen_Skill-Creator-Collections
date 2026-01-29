---
name: Test Plan Generator
description: Generates a complete Software Test Plan document based on project details.
---

# Test Plan Generator Skill

This skill is designed to assist users in creating a comprehensive Software Test Plan. It ensures all necessary details are gathered before generating a structured document, while allowing for smart defaults when minimal information is provided.

## Capabilities

1.  **Information Gathering**: Parses user input for project details.
2.  **Smart Defaults**: intelligently fills in missing non-critical information based on the project type.
3.  **Test Plan Generation**: Creates a formatted Markdown Test Plan.

## Workflow

1.  **Analyze Request**: When the user requests a test plan, check for the following information:
    *   **Project / Application Name** (e.g., E-Commerce Web App)
    *   **Application Type** (Web, Mobile, Desktop, API, etc.)
    *   **Business Objective** (Why the application is being built)
    *   **Key Features / Modules** (Login, Search, Payment, Reports, etc.)
    *   **In-Scope Functionalities** (What will be tested)
    *   **Out-of-Scope Functionalities** (What will NOT be tested)
    *   **Testing Types Required** (Functional, Regression, Smoke, Performance, Security, etc.)
    *   **Test Environment Details** (OS, Browser, Device, Build URL, Database)
    *   **Test Tools** (Selenium, Cypress, JMeter, Postman, etc.)
    *   **Test Data Requirements** (Dummy users, payment data, sample records)
    *   **Entry Criteria** (Conditions to start testing)
    *   **Exit Criteria** (Conditions to stop testing)
    *   **Team & Roles** (QA Lead, QA Engineers, Dev, Product Owner)
    *   **Timeline / Milestones** (Testing start & end dates)
    *   **Risks & Constraints** (Dependencies, unstable builds, limited environments)

2.  **Validate Input**:
    *   **Mandatory Fields**: Ensure the following are present:
        1.  **Project Name**
        2.  **Application Type**
        3.  **Key Features**
    *   **Action**: If any of these *three mandatory fields* are missing, **ask the user** for them immediately. Do not proceed until these are known.

3.  **Apply Smart Defaults**:
    *   If the user provides the *Mandatory Fields* but omits others (e.g., Test Tools, Test Environment, Entry/Exit Criteria), **assume reasonable defaults** based on the *Application Type* and *Key Features*.
    *   *Example*: If Application Type is "Web App", assume "Chrome/Firefox" for browsers and "Selenium/Playwright" for tools if not specified.

4.  **Generate Document**: Generate the Test Plan using the template below.

## Test Plan Template

```markdown
# Test Plan: <Project Name>

**Application Type:** <Application Type>
**Test Plan ID:** <Generated ID>

## 1. Business Objective
<Business Objective>

## 2. Scope
### Key Features / Modules
*   <Feature 1>
*   <Feature 2>

### In-Scope Functionalities
*   <Item>

### Out-of-Scope Functionalities
*   <Item>

## 3. Test Strategy
<Approach to testing based on application type>

## 4. Test Types
*   <Test Type 1>
*   <Test Type 2>

## 5. Test Environment
<OS, Browser, Device, Build URL, Database>

## 6. Test Data Requirements
<Data needs>

## 7. Test Tools
<List of tools>

## 8. Entry Criteria
*   <Criteria>

## 9. Exit Criteria
*   <Criteria>

## 10. Team & Roles
| Role | Responsibility |
| :--- | :--- |
| <Role> | <Description> |

## 11. Timeline / Milestones
| Milestone | Start Date | End Date |
| :--- | :--- | :--- |
| <Phase> | <Date> | <Date> |

## 12. Risks & Constraints
| Risk/Constraint | Mitigation/Handling |
| :--- | :--- |
| <Risk> | <Strategy> |

## 13. Deliverables
*   Test Plan Document
*   Test Cases / Scenarios
*   Defect Reports
*   Test Summary Report

## 14. Approval
| Name | Role | Signature | Date |
| :--- | :--- | :--- | :--- |
| <Name> | Key Stakeholder | | |
```
