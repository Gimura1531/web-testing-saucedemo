## BUG-01: Login error message is not user-friendly

- Environment:

Browser: Google Chrome
OS: macOS / Windows
URL: https://www.saucedemo.com/

- Steps to Reproduce:

Open the login page
Enter invalid credentials (e.g., username: wrong_user, password: wrong_pass)
Click "Login"

- Expected Result:

A clear and user-friendly error message is displayed (e.g., "Invalid username or password")

- Actual Result:

Error message displayed:
"Epic sadface: Username and password do not match any user in this service"

- Type: UX Issue / Improvement
Severity: Low
Priority: Low

- Screenshot:
  ![Login with invalid password](./screenshots/TC_02_invalid_pasword_name.png)

## BUG-02: Checkout form allows invalid data without validation

- Environment:

Browser: Google Chrome
OS: macOS / Windows
URL: https://www.saucedemo.com/

- Steps to Reproduce:

Log in with valid credentials (username: standard_user, password: secret_sauce)
Add any product to the cart
Open the cart and click "Checkout"
Enter invalid data:
First Name: 12345
Last Name: @@@@
Zip Code: abcde
Click "Continue"

- Expected Result:

Form validation should prevent submission
First Name and Last Name should accept only alphabetic characters
Zip Code should accept only numeric values
Validation error messages should be displayed

- Actual Result:

The system allows submission of invalid data
User is redirected to the checkout overview page

Type: Functional Bug
Severity: Medium
Priority: Medium

- Screenshot:
  ![Checkout Validation](./screenshots/bug_checkout_validation.png)
  ![Checkout Validation](./screenshots/TC_13_checkout_overview.png)