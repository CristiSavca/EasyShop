# E-Commerce API: EasyShop
___
This project is an e-commerce application or online store for a company called
EasyShop. 
## Overview
___
Web Application Features:
* List of items for sale
* Filter options(Category, Price, Color)
* Ability to add items to cart
* Header Options(Home,Profile,View Cart, Login/Logout)

To run application, the front end component (EasyShopFrontEnd) is required to format the website 
and the information sent by the backend portion.


### Phase 1 -  CategoriesController:
___
Phase 1 required implementing the methods inside the CategoriesController 
and MySqlCategoryDao class while assigning the proper annotations to the controller. 

List of implemented methods:
* getAll()
* getById()
* getProductsById()
* addCategory()
* updateCategory()
* deleteCategory()

REST methods required:

![img](https://github.com/CristiSavca/EasyShop/assets/58373811/c5c4c009-4dc4-4c06-82b8-21dbe7ef26df)

CategoriesController addCategory() method implementation:
![img_1](https://github.com/CristiSavca/EasyShop/assets/58373811/4a11608b-87b3-425b-b152-2f5216efa44c)

MySqlCategoryDao create() method implementation:

![img_2](https://github.com/CristiSavca/EasyShop/assets/58373811/ec3f1eff-a2ce-49b2-93b7-17248cb1a5aa)

### Phase 2 -  Fix Bugs:
___

For bug 1, the product search functionality is returning incorrect results.
All that was required to fix this bug was to add a maximum price line in 
the sql statement. The maxPrice was also added twice inside the try/catch code.

![img_3](https://github.com/CristiSavca/EasyShop/assets/58373811/ce4c9a02-96da-4b42-ad9e-9d4170b19aaf)

For bug 2, products would be duplicated because instead of updating the product,
a new product would be added to the database. To fix this all that was required was to
change create to update in below method.

![img_4](https://github.com/CristiSavca/EasyShop/assets/58373811/e6bf18b4-4a2c-4d19-ba25-bedc4526d258)

## Interesting Piece of Code
___

MySqlCategoryDaoTest:

![img_5](https://github.com/CristiSavca/EasyShop/assets/58373811/c0395841-c05a-4f05-a1a3-2dd0f5c82209)

