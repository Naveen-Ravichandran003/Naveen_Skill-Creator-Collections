# Selenium Java Code Reviewer Skill

## Description
Reviews Selenium automation code written in Java. The skill analyzes the code for quality, best practices, and potential issues, providing constructive and actionable feedback.

## Required Inputs
The user must provide:
1. **Code Snippet**
   - Selenium automation code written in Java.
   - Can include test classes, page objects, or framework utilities.
2. **Code Purpose**
   - What the code is intended to do.
   - Example: "Login test automation", "Page Object for Checkout page".

*If any required input is missing, ask the user before performing the review.*

## Optional Inputs
- **Framework Type**
  - Example: TestNG, JUnit, Cucumber
- **Focus Area**
  - Default: Code Quality and Best Practices
  - Options:
    - Code Quality
    - Framework Design
    - Performance
    - Readability
    - Best Practices
    - Error Handling
- **Desired Output Detail Level**
  - Default: Medium
  - Options: Short, Medium, Detailed

## Validation Rules
- **Must** verify that the provided code is Java-based Selenium before reviewing. If not, ask the user to provide correct code.
- **Must not** review code if `Code Snippet` is missing.
- **Must not** rewrite full code unless user requests refactoring.
- **Must not** claim execution or runtime testing of code.
- **Must** keep feedback constructive and actionable.

## Output Rules
- **Structure**:
  - Identify strengths in the code.
  - List improvement suggestions.
  - Highlight potential bugs or risks.
  - Provide best-practice recommendations.
- **Severity Labels**:
  - Label issues as:
    - **[Critical]**: May cause failures.
    - **[Improvement]**: Code enhancement.
    - **[Suggestion]**: Nice-to-have.
- **Format**:
  - Use bullet points.
  - **Do not use tables**.
