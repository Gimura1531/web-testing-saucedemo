# Test Cases - SauceDemo

---

### TC-01: Login with valid credentials

ID: TC-01
Title: Verify user login with valid credentials

Preconditions:

Login page is opened

Steps:

Enter username: standard_user
Enter password: secret_sauce
Click "Login"

Postconditions:

User is logged out

Expected Result:

User is redirected to the products page

Actual Result:

User successfully logged in and redirected

Status:

Passed

- Screenshot:
  ![Login](./screenshots/TC_01_login.png)
  ![Login Success](./screenshots/TC_01_success_login.png)
---

- Steps:
### TC-02: Login with invalid password

ID: TC-02
Title: Verify login with invalid credentials

Preconditions:

Login page is opened

Steps:

Enter username: wrong_username
Enter password: wrong_password
Click "Login"

Postconditions:

None

Expected Result:

Error message is displayed

Actual Result:

Error message displayed

Status:

Passed

- Screenshot:
  ![Login with invalid password](./screenshots/TC_02_invalid_pasword_name.png)
---

### TC-03: Login with empty fields

ID: TC-03
Title: Verify login with empty fields

Preconditions:

Login page is opened

Steps:

Leave username empty
Leave password empty
Click "Login"

Postconditions:

None

Expected Result:

Validation error is displayed

Actual Result:

Error message displayed

Status:

Passed

- Screenshot:
  ![Login with empty fields](./screenshots/TC_03_empty_fields.png)
---

### TC-04: Login with locked user

ID: TC-04
Title: Verify login with locked user

Preconditions:

Login page is opened

Steps:

Enter username: locked_out_user
Enter password: secret_sauce
Click "Login"

Postconditions:

None

Expected Result:

Error message about locked user

Actual Result:

Error message displayed

Status:

Passed

- Screenshot:
  ![Login with locked user](./screenshots/TC_04_locked_user.png)
---

### TC-05: Logout functionality

ID: TC-05
Title: Verify logout functionality

Preconditions:

User is logged in

Steps:

Open menu
Click "Logout"

Postconditions:

User remains logged out

Expected Result:

User is redirected to login page

Actual Result:

User returned to login page

Status:

Passed

- Screenshot:
  ![Logout functionality](./screenshots/TC_05_logout.png)
---

### TC-06: Add product to cart

ID: TC-06
Title: Verify adding product to cart

Preconditions:

User is logged in

Steps:

Click "Add to cart"

Postconditions:

Remove item from cart

Expected Result:

Button changes to "Remove"
Cart icon shows 1 item

Actual Result:

Product added successfully

Status:

Passed

- Screenshot:
  ![Add product to cart](./screenshots/TC_06_add_product.png)
---

### TC-07: Remove product from cart

ID: TC-07
Title: Verify removing product from cart

Preconditions:

Product is added to cart

Steps:

Click "Remove"

Postconditions:

None

Expected Result:

Product removed from cart
Cart count updated

Actual Result:

Product removed successfully

Status:

Passed

- Screenshot:
  ![Remove product from cart](./screenshots/TC_07_remove_product_1.png)
  ![Remove product from cart](./screenshots/TC_07_remove_product_2.png)
---

### TC-08: Open product details

ID: TC-08
Title: Verify opening product details

Preconditions:

User is logged in

Steps:

Click on product name

Postconditions:

Return to products page

Expected Result:

Product details page opens

Actual Result:

Product page displayed

Status:

Passed

- Screenshot:
  ![Open product details](./screenshots/TC_08_product_details.png)
---

### TC-09: Sort products by price (low to high)

ID: TC-09
Title: Verify sorting products by price (low to high)

Preconditions:

User is on products page

Steps:

Select sorting option "Price (low to high)"

Postconditions:

None

Expected Result:

Products sorted by ascending price

Actual Result:

Sorting works correctly

Status:

Passed

- Screenshot:
  ![Sort products by price](./screenshots/TC_09_sort_products_by_price.png)
---

### TC-10: Add multiple products to cart

ID: TC-10
Title: Verify adding multiple products to cart

Preconditions:

User is logged in

Steps:

Add 1-2 products

Postconditions:

Remove products from cart

Expected Result:

Cart shows correct number of items

Actual Result:

Items added correctly

Status:

Passed

- Screenshot:
  ![Add multiple products to cart](./screenshots/TC_10_multiple_products.png)
---

### TC-11: Open cart page

ID: TC-11
Title: Verify opening cart page

Preconditions:

User is logged in

Steps:

Click cart icon

Postconditions:

Return to products page

Expected Result:

Cart page is displayed

Actual Result:

Cart opened successfully

Status:

Passed

- Screenshot:
  ![Open cart page](./screenshots/TC_11_open_cart_page.png)
---

### TC-12: Continue shopping from cart

ID: TC-12
Title: Verify continue shopping from cart

Preconditions:

User is in cart

Steps:

Click "Continue Shopping"

Postconditions:

None

Expected Result:

User returns to products page

Actual Result:

Navigation works correctly

Status:

Passed

- Screenshot:
  ![Continue shopping from cart](./screenshots/TC_12_continue_shopping.png)
---

### TC-13: Checkout process (basic)

ID: TC-13
Title: Verify checkout process

Preconditions:

Product is in cart

Steps:

Click "Checkout"
Enter First Name
Enter Last Name
Enter Zip code
Click "Continue"

Postconditions:

Order not completed

Expected Result:

User proceeds to checkout overview

Actual Result:

Navigation successful

Status:

Passed

- Screenshot:
  ![Checkout process](./screenshots/TC_13_checkout_proccess.png)
  ![Checkout overview](./screenshots/TC_13_checkout_overview.png)
---

### TC-14: Checkout with empty fields

ID: TC-14
Title: Verify checkout with empty fields

Preconditions:

User is on checkout page

Steps:

Leave fields empty
Click "Continue"

Postconditions:

None

Expected Result:

Validation error displayed

Actual Result:

Error message shown

Status:

Passed

- Screenshot:
  ![Checkout with empty fields](./screenshots/TC_14_checkout_empty.png)
---

### TC-15: Finish order

ID: TC-15
Title: Verify order completion

Preconditions:

User is on checkout overview page

Steps:

Click "Finish"

Postconditions:

User returned to main page

Expected Result:

Order success message displayed

Actual Result:

Order completed successfully

Status:

Passed

- Screenshot:
  ![Finish order](./screenshots/TC_15_finish.png)