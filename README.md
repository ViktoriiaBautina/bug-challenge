# Paylocity Bug Challenge 

URL and Login info: https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login

API Documentation:
The API documentation can be found at the below link: https://documenter.getpostman.com/view/2314100/SWTEbbi6


**User Story**:

As an Employer, I want to input my employee data so that I can get a preview of benefit costs.

**Acceptance Criteria**

**Scenario 1: Add Employee**

GIVEN an Employer
AND I am on the Benefits Dashboard page
WHEN I select Add Employee
THEN I should be able to enter employee details
AND the employee should save
AND I should see the employee in the table
AND the benefit cost calculations are correct

**Scenario 2: Edit Employee**

GIVEN an Employer
AND I am on the Benefits Dashboard page
WHEN I select the Action Edit
THEN I can edit employee details
AND the data should change in the table

**Scenario 3: Delete Employee**

GIVEN an Employer
AND I am on the Benefits Dashboard page
WHEN I click the Action X
THEN the employee should be deleted

The reported bugs can be found in the following file: bug_challenge.md
