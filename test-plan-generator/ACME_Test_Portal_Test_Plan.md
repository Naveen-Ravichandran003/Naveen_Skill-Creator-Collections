# Test Plan: ACME Test Portal

**Application Type:** Web Application
**Test Plan ID:** TP-ACME-001

## 1. Business Objective
Provide a stable and reliable demo web portal that allows users developers to practice and demonstrate UI automation testing capabilities effectively.

## 2. Scope
### Key Features / Modules
*   User Login & Authentication
*   Dashboard Navigation
*   Form Submissions
*   Table Data Handling (extraction, sorting, filtering)
*   Alerts & Pop-ups Handling
*   File Upload Functionality

### In-Scope Functionalities
*   Verification of all UI elements and interactions on the key features listed above.
*   Validation of positive and negative scenarios for forms and login.
*   Cross-browser compatibility (Chrome, Firefox).

### Out-of-Scope Functionalities
*   Performance / Load Testing
*   Security / Penetration Testing
*   API Testing (unless directly related to UI actions)
*   Mobile responsive testing (Desktop view priority)

## 3. Test Strategy
The testing approach will focus on verifying the functional correctness of the web portal's UI components. Automation will be prioritized using Selenium WebDriver to ensure repeatable regression testing. Manual exploratory testing will be conducted for initial feature validation and usability.

## 4. Test Types
*   Functional Testing
*   UI Testing
*   Smoke Testing
*   Regression Testing

## 5. Test Environment
*   **URL:** https://acme-test.uipath.com
*   **OS:** Windows 10/11
*   **Browsers:** Google Chrome (Latest), Mozilla Firefox (Latest)
*   **Network:** Standard Broadband/Enterprise Network

## 6. Test Data Requirements
*   Dummy User Credentials (Valid/Invalid username & passwords)
*   Sample values for form fields (Alphanumeric, Special chars)
*   Sample files for upload testing (.txt, .pdf, .csv)

## 7. Test Tools
*   **Automation:** Selenium WebDriver with Java
*   **Framework:** TestNG
*   **IDE:** IntelliJ IDEA / Eclipse
*   **Build Tool:** Maven/Gradle (Assumed)

## 8. Entry Criteria
*   Test Environment (URL) is accessible.
*   Smoke test cases passed successfully.
*   Valid test credentials are provided.
*   Test Plan approved.

## 9. Exit Criteria
*   100% of critical and high-priority test cases executed.
*   Pass rate of >95% for executed test cases.
*   No open Critical (P1) or High (P2) severity defects.
*   Regression suit execution completed.

## 10. Team & Roles
| Role | Responsibility |
| :--- | :--- |
| **QA Lead** | Test planning, Strategy definition, Review |
| **QA Engineer** | Test case creation, Automation scripting, Execution, Bug Reporting |
| **Developer** | Bug fixing, Unit testing |

## 11. Timeline / Milestones
| Milestone | Start Date | End Date |
| :--- | :--- | :--- |
| Test Planning | TBD | TBD |
| Test Case Design | TBD | TBD |
| Execution (Smoke) | TBD | TBD |
| Execution (Regression) | TBD | TBD |
| Sign-off | TBD | TBD |

## 12. Risks & Constraints
| Risk/Constraint | Mitigation/Handling |
| :--- | :--- |
| Application Downtime | Plan testing during stable hours; coordinate with Dev ops. |
| UI Changes | Use robust locators (ID, CSS) to minimize maintenance; communicate with Devs. |
| Limited Test Data | Generate scripts to create reusable test data. |

## 13. Deliverables
*   Test Plan Document
*   Test Cases / Scenarios
*   Defect Reports
*   Test Summary Report / Execution Logs

## 14. Approval
| Name | Role | Signature | Date |
| :--- | :--- | :--- | :--- |
| [Name] | Project Manager | | |
| [Name] | QA Manager | | |
