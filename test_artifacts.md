**Test Plan**

_Objectives_: 
1. To verify the login functionality by testing for both valid and invalid credential input.
2. To confirm if the proper redirects are executed upon successful login as well as if user-friendly error messages are displayed on incorrect login.

_Scope_: 
The test covers the Login page of the application. The functional areas under test include input fields of 'Email' and 'Password', 'Login' button, redirect upon successful login, and displayed error messages. 

_Responsibilities_: 
All testing-related activities will be conducted by the QA team. Developers will rectify defects identified during testing. 

**User Scenarios**

_Scenario 1: Successful Login_
1. User navigates to the Login page.
2. User enters valid Email and Password.
3. User clicks the 'Login' button.
4. System verifies the credentials.
5. Upon verification, user is redirected to their Dashboard.

_Scenario 2: Unsuccessful Login_
1. User navigates to the Login page.
2. User enters invalid Email and/or Password.
3. User clicks the 'Login' button.
4. System verifies the credentials.
5. Since details are invalid, an error message is displayed to the user.

**Test Data**

_Valid Data_
1. Email: user@example.com | Password: password123 

_Invalid Data_
1. Email: user@example.com | Password: wrongpassword 
2. Email: wronguser@example.com | Password: password123
3. Email: wronguser@example | Password: wrongpassword
4. Email: '' (empty) | Password: password123
5. Email: user@example.com | Password: '' (empty)
6. Invalid email formats (user@example, 123abcd, user@.com)

_ERROR MESSAGES_
1. For invalid email: 'Invalid email. Please check the entered email.'
2. For invalid password: 'Invalid password. Please check the entered password.'
3. For both invalid: 'Invalid email and password. Please check the entered details.'