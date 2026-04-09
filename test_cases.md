# Test Cases - SauceDemo

---

### TC-01: Login with valid credentials
- Preconditions: Открыта страница логина
- Steps:
  1. Ввести username: standard_user
  2. Ввести password: secret_sauce
  3. Нажать кнопку Login
- Expected result:
  Пользователь успешно входит и попадает на страницу товаров
- Screenshot:
  ![Login](./screenshots/TC_01_login.png)
  ![Login Success](./screenshots/TC_01_success_login.png)
---

### TC-02: Login with invalid password
- Preconditions: Открыта страница логина
- Steps:
  1. Ввести username: wrong_username
  2. Ввести password: wrong_password
  3. Нажать Login
- Expected result:
  Появляется сообщение об ошибке
- Screenshot:
  ![Login with invalid password](./screenshots/TC_02_invalid_pasword_name.png)
---

### TC-03: Login with empty fields
- Preconditions: Открыта страница логина
- Steps:
  1. Оставить поля пустыми
  2. Нажать Login
- Expected result:
  Появляется ошибка о необходимости ввода данных
- Screenshot:
  ![Login with empty fields](./screenshots/TC_03_empty_fields.png)
---

### TC-04: Login with locked user
- Preconditions: Открыта страница логина
- Steps:
  1. Ввести username: locked_out_user
  2. Ввести password: secret_sauce
  3. Нажать Login
- Expected result:
  Появляется сообщение, что пользователь заблокирован
- Screenshot:
  ![Login with locked user](./screenshots/TC_04_locked_user.png)
---

### TC-05: Logout functionality
- Preconditions: Пользователь залогинен
- Steps:
  1. Открыть меню (бургер)
  2. Нажать Logout
- Expected result:
  Пользователь возвращается на страницу логина
- Screenshot:
  ![Logout functionality](./screenshots/TC_05_logout.png)
---

### TC-06: Add product to cart
- Preconditions: Пользователь залогинен
- Steps:
  1. Нажать "Add to cart" у любого товара
- Expected result:
  Кнопка меняется на "Remove"
  Иконка корзины показывает 1 товар
- Screenshot:
  ![Add product to cart](./screenshots/TC_06_add_product.png)
---

### TC-07: Remove product from cart
- Preconditions: Товар добавлен в корзину
- Steps:
  1. Нажать "Remove"
- Expected result:
  Товар удаляется из корзины
  Счетчик уменьшается
- Screenshot:
  ![Remove product from cart](./screenshots/TC_07_remove_product_1.png)
  ![Remove product from cart](./screenshots/TC_07_remove_product_2.png)
---

### TC-08: Open product details
- Preconditions: Пользователь залогинен
- Steps:
  1. Нажать на название товара
- Expected result:
  Открывается страница с деталями товара
- Screenshot:
  ![Open product details](./screenshots/TC_08_product_details.png)
---

### TC-09: Sort products by price (low to high)
- Preconditions: Пользователь на странице товаров
- Steps:
  1. Выбрать сортировку "Price (low to high)"
- Expected result:
  Товары отсортированы по возрастанию цены
- Screenshot:
  ![Sort products by price](./screenshots/TC_09_sort_products_by_price.png)
---

### TC-10: Add multiple products to cart
- Preconditions: Пользователь залогинен
- Steps:
  1. Добавить 2-3 товара
- Expected result:
  В корзине отображается правильное количество товаров
- Screenshot:
  ![Add multiple products to cart](./screenshots/TC_10_multiple_products.png)
---

### TC-11: Open cart page
- Preconditions: Пользователь залогинен
- Steps:
  1. Нажать на иконку корзины
- Expected result:
  Открывается страница корзины с добавленными товарами
- Screenshot:
  ![Open cart page](./screenshots/TC_11_open_cart_page.png)
---

### TC-12: Continue shopping from cart
- Preconditions: Пользователь в корзине
- Steps:
  1. Нажать "Continue Shopping"
- Expected result:
  Пользователь возвращается к списку товаров
- Screenshot:
  ![Continue shopping from cart](./screenshots/TC_12_continue_shopping.png)
---

### TC-13: Checkout process (basic)
- Preconditions: В корзине есть товар
- Steps:
  1. Нажать Checkout
  2. Ввести First Name, Last Name, Zip
  3. Нажать Continue
- Expected result:
  Переход на страницу подтверждения заказа
- Screenshot:
  ![Checkout process](./screenshots/TC_13_checkout_proccess.png)
  ![Checkout overview](./screenshots/TC_13_checkout_overview.png)
---

### TC-14: Checkout with empty fields
- Preconditions: Пользователь на этапе Checkout
- Steps:
  1. Оставить поля пустыми
  2. Нажать Continue
- Expected result:
  Появляется ошибка о незаполненных полях
- Screenshot:
  ![Checkout with empty fields](./screenshots/TC_14_checkout_empty.png)
---

### TC-15: Finish order
- Preconditions: Пользователь на финальном шаге Checkout
- Steps:
  1. Нажать Finish
- Expected result:
  Появляется сообщение об успешном заказе
- Screenshot:
  ![Finish order](./screenshots/TC_15_finish.png)