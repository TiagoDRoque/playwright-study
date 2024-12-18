
#Test Plans 

## **1. Introduction**

   - **Goal:** The main goal of these test cases is to verify the functionality and reliability of the login system, product search, and checkout processes.

## **2. The strategy**

  - **Manual Testing:** Focus on exploratory testing for new features.
  - **Automated Testing:** Functional testing using Playwright to verify that:
    - Core features work as expected under various conditions.
    - Automated scripts provide consistent and reliable test coverage, reducing manual effort over time.

  - **Tools:** Playwright.

## **Environment Details**
- **Base URL:** `https://www.saucedemo.com/`
- **Test Users:**
  - `standard_user`
  - `locked_out_user`
  - `problem_user`
  - `performance_glitch_user`
  - `error_user`
  - `visual_user`

- **Test Password:**
  - `secret_sauce`

### **Notes:**
  - This project is intended for **study purposes**, so it's acceptable to include data directly in the document. 
  - However, in an **official project**, sensitive data such as passwords should never be included in documentation or source code.
  - For official projects:
    - Store credentials securely in a configuration file (e.g., `.env`) or as environment variables.
    - Use appropriate security practices to protect sensitive information.

