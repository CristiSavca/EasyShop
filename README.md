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

![image](https://github.com/CristiSavca/EasyShop/assets/58373811/66983767-28f0-4a83-bf2b-9728d3a93424)


CategoriesController addCategory() method implementation:
![image](https://github.com/CristiSavca/EasyShop/assets/58373811/0a83ee5b-58fc-4438-8536-035ac352d30b)


MySqlCategoryDao create() method implementation:

![image](https://github.com/CristiSavca/EasyShop/assets/58373811/9fe160dc-cd9c-4036-9c00-7470c5aacbf3)

### Phase 2 -  Fix Bugs:
___

For bug 1, the product search functionality is returning incorrect results.
All that was required to fix this bug was to add a maximum price line in 
the sql statement. The maxPrice was also added twice inside the try/catch code.

![image](https://github.com/CristiSavca/EasyShop/assets/58373811/a91db119-7f2a-45d4-91f3-9e124f99545d)

For bug 2, products would be duplicated because instead of updating the product,
a new product would be added to the database. To fix this all that was required was to
change create to update in below method.

![image](https://github.com/CristiSavca/EasyShop/assets/58373811/4bb57e07-baf3-4a79-b48a-57cdc6dd6fbc)

## Interesting Piece of Code
___

MySqlCategoryDaoTest:

![image](https://github.com/CristiSavca/EasyShop/assets/58373811/630d940a-8795-42d6-b19c-781184d0c563)

