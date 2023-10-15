

**ID: 01 Summary** : The First name and the Last name - the column names are misplaced in the table

**Pre-conditions:**

1. Login to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login) with a valid credentials

Username: TestUser319

Password: M9KREpw#0-(c

**Description** :

**Steps to reproduce:**

1. Click on the "Add Employee" button;
2. Fill in First name field with the value "Mark;
3. Fill in Last name field with the value "Toy";
4. Click on the "Add" button

**Expected result:**

Toy is in the Last name column;

Mark is in the First name column;

**Actual result:**

Mark is in the Last name column;

Toy is in the First name column;

**Attachments:**

<img width="452" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%201.png">


**Severity** : Low

**Priority** : High

**Status** : Open

**Environment** :  macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023

<br> <br> **ID: 02 Summary** : There is no validation error/message when the Length of the First and Last Name is more than 50 symbols

**Pre-conditions:**

1. Login to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login) with valid credentials

Username: TestUser319

Password: M9KREpw#0-(c

**Description** :

When User fills in the Last name or First name fields more than 50 symbols, there is no notification/error message occurs.

I see in the response on Chrome devtools: "errorMessage": "The field FirstName must be a string with a maximum length of 50."

**Steps to reproduce:**

1. Click on the "Add Employee" button;
2. Fill in First name/Last name field with the value "Tonyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyy" (51 letter)
3. Fill in Last name/First name field with the value "Joe";
4. Click on the "Add" button

**Expected result:**

Validation message appears on UI describing that the field FirstName/Last name must be a string with a maximum length of 50.

**Actual result:**

No validation message appears on UI describing that the field FirstName/Last name must be a string with a maximum length of 50.

**Attachments:**

<img width="452" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%202.png">


**Severity** : Low

**Priority** : Medium

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023 

<br> <br> **ID: 03 Summary** : It is possible to use numbers and special symbols in Last Name and First name fields

**Pre-conditions:**

1. Login to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login) with a valid credentials

Username: TestUser319

Password: M9KREpw#0-(c

**Description** :

**Steps to reproduce:**

1. Click on the "Add Employee" button;
2. Fill in First name/Last name field with the value "Micha$e\*l5"
3. Fill in Last name/First name field with the value "L!)eo3";
4. Click on the "Add" button

**Expected result:**

Impossible to submit adding a new employee form with numbers and special symbols in First name/Last name fields;

**Actual result:**

It is allowed to submit adding a new employee form with numbers and special symbols in First name/Last name fields;

**Attachments:**

<img width="452" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%203.png">


**Severity** : Low

**Priority** : Medium

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023

<br> <br> **ID: 04 Summary** : Internal server error occurs when Dependants field contains letters or special character

**Pre-conditions:**

1. Login to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login) with a valid credentials

Username: TestUser319

Password: M9KREpw#0-(c

**Description** :

**Steps to reproduce:**

1. Click on the "Add Employee" button;
2. Fill in First name field with the value "Leo"
3. Fill in Last name field with the value "Nell"
4. Fill in Dependants field with the value no number – string or special character
5. Click on the "Add" button

**Expected result:**

Validation message occurs explaining that Dependants is a number between 0 and 32;

**Actual result:**

500 Internal Server Error.

**Attachments:**

<img width="452" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%204.png">

**Severity** : High

**Priority** : High

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023

<br> <br> **ID: 05 Summary** : Automatic logout after 30 minutes user being logged in without any notification

**Pre-conditions:**

1. Login to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login) with a valid credentials

Username: TestUser319

Password: M9KREpw#0-(c

**Description** : User is performing actions and unexpectedly logout after 30 minutes being logged in.

**Steps to reproduce:**

1. Be active for 30 mins;

**Expected result:**

I as a User will not be logged out when I am performing actions (Add, Update or Delete Employees) or the notification message occurs before logout.

**Actual result:**

There is not any notification message about future logout. Error 401 Unauthorized occurs in Chrome devtools.

**Attachments:**

<img width="452" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%205.png">


**Severity** : Low

**Priority** : Medium

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023

<br> <br> **ID: 06 Summary** : After logout, there is no visible actions on UI e.g. redirections on a Login page or notification

**Pre-conditions:**

1. Login to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login) with a valid credentials

Username: TestUser319

Password: M9KREpw#0-(c

**Description** :

**Steps to reproduce:**

1. Be active for 30 mins;

**Expected result:**

User is redirected to the Login page after being logged out or notification message occurs.

**Actual result:**

After logout, there are no visible actions on UI (e.g. redirections on Login page or notification describing that user was logged out and it is needed to click on "Log Out" manually.

**Severity** : Medium

**Priority** : Medium

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023

<br> <br> **ID: 07 Summary** : A new created Employee record is displayed  in random place in the table

**Pre-conditions:**

1. Login to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login) with a valid credentials

Username: TestUser319

Password: M9KREpw#0-(c

**Description** :

**Steps to reproduce:**

1. Add a few new Employee records

**Expected result:**

The order for recently created records is consistent (e.g. at the top, at the bottom)

**Actual result:** There is no consistent order to place a new created record. Sometimes a new element is displayed at the top, sometimes in the middle or at the bottom.

**Severity** : Low

**Priority** : Medium

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023

<br> <br> **ID: 08 Summary** : Favicon isn't loaded with error 403 (Forbidden) 

**Pre-conditions:**

1. Login to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login) with a valid credentials

Username: TestUser319

Password: M9KREpw#0-(c

**Description** :

**Steps to reproduce:**

1. Refresh the page by clicking on the header "Paylocity Benefits Dashboard"
2. Check the Chrome devtools console

**Expected result:** Favicon is loaded

**Actual result:** Favicon isn't loaded with error 403 (Forbidden) 

**Attachments:**

<img width="452" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%208.png">

**Severity** : Low

**Priority** : Low

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023

<br> <br> **ID: 09 Summary** : Error 500 occurs when logging in with an invalid Username

**Description** :

**Steps to reproduce:**

1. Navigate to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login)
2. Fill in Username with invalid data;
3. Fill in a valid Password;
4. Click the "Log In" button.

**Expected result:**

The error message occurs: "There were one or more problems that prevented you from logging in:

- The specified username or password is incorrect."

**Actual result:**

500 Internal Server error occurs.

**Attachments:**

<img width="452" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%209.png">

**Severity** : High

**Priority** : High

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023

<br> <br> **ID: 10 Summary** : Possible to see the content without a login when clicking on "Paylocity Benefits Dashboard"

**Description** :

**Steps to reproduce:**

1. Navigate to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login)
2. Click on the header at the top of the page "Paylocity Benefits Dashboard"

**Expected result: "** Paylocity Benefits Dashboard" is refreshing the login page.

**Actual result:**

It is possible to see a table header, "Add" button and Add Employee form without logging in

**Attachments:**

<img width="452" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%2010(1).png">

<img width="330" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%2010(2).png">


**Severity** : High

**Priority** : High

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023

<br> <br> **ID: 11 Summary** : API: Error 500 occurs when sending a request to GET Employee with a non-existent ID

**Description** : Send a request to GET Employee with a non-existent ID

**Steps to reproduce:**

1. Send a POST to create an employee;
2. Check the response;
3. Copy the ID of created employee;
4. Send a GET employee request adding the ID from the step 3 and delete the last symbol;

**Expected result:**

The error 404Not Found occurs.

**Actual result:**

The Internal Server error 500 occurs.

**Attachments:**

<img width="452" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%2011.png">


**Severity** : High

**Priority** : High

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149; Postman for Web Version 10.19.2-231013-1449

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 13/10/2023


<br> <br> **ID: 12 Summary** : API: The benefit cost calculations are not correct in the response of PUT request

**Description** :

**Steps to reproduce:**

1. Send a PUT request https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/api/employees

Headers:

Content-Type application/json

Authorization Basic VGVzdFVzZXIzMTk6TTlLUkVwdyMwLShj

With a body:

```json
{

"id":"1945d706-39f3-49eb-bea8-98abcf766e5e",

"firstName":"Wanda",

"lastName":"Maximoff",

"dependants":2

}
```

**Expected result:**
```json
{
"partitionKey": "TestUser319",
    "sortKey": "a23eb306-8f31-4991-b00b-97e0c818fdd6",
    "username": "TestUser319",
    "id": "a23eb306-8f31-4991-b00b-97e0c818fdd6",
    "firstName": "Wanda",
    "lastName": "Maximoff",
    "dependants":2,
    "salary":52000.0,
    "gross":2000.0,
    "benefitsCost":76.92308,
    "net":1923.0769
}
```

**Actual result:** The salary and gross are 0.0 and calculations are not correct
```json

{
"partitionKey": "TestUser319",
    "sortKey": "a23eb306-8f31-4991-b00b-97e0c818fdd6",
    "username": "TestUser319",
    "id": "a23eb306-8f31-4991-b00b-97e0c818fdd6",
    "firstName": "Wanda",
    "lastName": "Maximoff",
    "dependants":2,
    "salary":0.0,
    "gross":0.0,
    "benefitsCost":76.92308,
    "net":-76.92308
}
```

**Severity** : Medium

**Priority** : High

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149; Postman for Web Version 10.19.2-231013-1449

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 14/10/2023

<br> <br> **ID: 13 Summary** : API: It is possible to send a DELETE many times with the same ID

**Steps to reproduce:**

1. Send DELETE method with an existing ID
2. Repeat step 1 a few times

**Expected result:**

After the first request, the record is deleted. The error 404Not Found should be returned.

**Actual result:**

Status code is 200 OK. No errors occur.

**Attachments:**

**Severity** : Medium

**Priority** : Medium

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149; Postman for Web Version 10.19.2-231013-1449

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 14/10/2023

<br> <br> **ID: 14 Summary** : Security Vulnerability: It is allowed to log in to Stage environment when changing Stage instead of Prod on this path: https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login

**Description** : It is allowed to log in to Stage environment with a Prod valid credentials

**Steps to reproduce:**

1. Go to [https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login](https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Prod/Account/Login)
2. Open the devtools;
3. Check employeeClient.js. In the code there's a condition for prod and stage envs;
4. Navigate to https://wmxrwq14uc.execute-api.us-east-1.amazonaws.com/Stage/Account/Login
5. Fill in valid credentials;
6. Click "Log In" button

**Expected result:** It is forbidden to login to Stage environment and make some changes there (Add new employee, edit and delete employee).

**Actual result:** It is possible to login to Stage env, see the content and perform actions with the credentials for Prod.

**Attachments**:

<img width="365" alt="image" src="https://github.com/ViktoriiaBautina/bug-challenge/blob/main/images/Picture%2014.png">

**Severity** : Highest

**Priority** : Highest

**Status** : Open

**Environment** : macOS 13.3.1 (a) (22E772610a), Google Chrome Version 117.0.5938.149

**Assignee** :

**Reporter** : Viktoriia Bautina

**Date** : 14/10/2023
