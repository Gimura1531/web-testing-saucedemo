## BUG-01: Checkout form allows invalid data without validation

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