#Login Test Cases

## **Test Casse - Verify the 'standard_user' logged in successfully and the system redirects to the HomePage**
- **Precondition**:
  1. The user has access to the login page.
- **Steps**:
  1. Open the login page
  2. Fill the "username" input with "standard_user"
  3. Fill the "password" input with ("secret_sauce")
  4. Click on "Login" button
- **Expect Result**:The system Home Page displayed

## **Test Casse - Verify the system displays an error message when "locked_out_user" attempts to log in .**
- **Precondition**:
  1. The user has access to the login page.
- **Steps**:
  1. Open the login page
  2. Fill the "username" input with "locked_out_user"
  3. Fill the "password" input with ("secret_sauce")
  4. Click on "Login" button
- **Expect Result**: 
  1. The system does not allow the user to log in.
  2. An error message is displayed on the login page with the following content:
   - `'Epic sadface: Sorry, this user has been locked out.'`
  3. The user remains on the login page.

## **Test Casse - Verify the system displays incorrect product images on the "Home Page" for "problem_user" .**
- **Precondition**:
  1. The user has access to the login page.
- **Steps**:
  1. Open the login page
  2. Fill the "username" input with "problem_user"
  3. Fill the "password" input with ("secret_sauce")
  4. Click on "Login" button
- **Expect Result**: 
  1. The system redirects the user to the "Home Page."
  2. On the Home Page, all of the displayed products have incorrect images

## **Test Casse - Verify the system displays an error message when the user enters an incorrect password.**
- **Precondition**:
  1. The user has access to the login page.
- **Steps**:
  1. Open the login page
  2. Fill the "username" input with "standard_user"
  3. Fill the "password" input with "wrong_password"
  4. Click on "Login" button
- **Expect Result**:
  1. The system does not allow the user to log in.
  2. An error message is displayed on the login page with the following content:
   - `'Epic sadface: Username and password do not match any user in this service.'`

## **Test Casse - Verify the user fills with the wrong username and the system displays an error message .**
- **Precondition**:
  1. The user has access to the login page.
- **Steps**:
  1. Open the login page
  2. Fill the "username" input with "standard_userr"
  3. Fill the "password" input with ("secret_sauce")
  4. Click on "Login" button
- **Expect Result**: The system display an error message,such as:('Epic sadface: Username and password do not match any user in this service.')

## **Test Casse - Verify the system displays an error message when the user enters an incorrect username.**
- **Precondition**:
  1. The user has access to the login page.
- **Steps**:
  1. Open the login page
  2. Click on "Login" button
- **Expect Result**:
  1. The system does not allow the user to log in.
  2. An error message is displayed on the login page with the following content:
   - `'Epic sadface: Username and password do not match any user in this service.'`

## **Test Case - Verify the system displays an error message when the user only fills the username input.**
- **Precondition**:
  1. The user has access to the login page.
- **Steps**:
  1. Open the login page
  2. Fill the "username" input with "standard_userr"
  3. Click on "Login" button
- **Expect Result**:
  1. The system does not allow the user to log in.
  2. An error message is displayed on the login page with the following content:
   - `'Epic sadface: Password is required.'`

## **Test Casse - Verify the system displays an error message when the user only fills the password input.**
- **Precondition**:
  1. The user has access to the login page.
- **Steps**:
  1. Open the login page
  2. Fill the "password" input with ("secret_sauce")
  3. Click on "Login" button
- **Expect Result**: 
  1. The system does not allow the user to log in.
  2. An error message is displayed on the login page with the following content:
   - `'Epic sadface: Username is required.'`

## **Test Casse - Verify the system displays the labels and inputs correctly on the login page.**
- **Precondition**:
  1. The user has access to the login page.
- **Steps**:
  1. Open the login page
- **Expect Result**:
  The login page displays the following elements correctly:
   - **Username input field**: Labeled correctly with the text "Username."
   - **Password input field**: Labeled correctly with the text "Password."
   - **Login button**: Labeled correctly with the text "Login."