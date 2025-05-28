# 1. E-Testing App
## 🧰 Tech Stack

- **Frontend:** React, Semantic UI  
- **Backend:** Node.js, Express.js (microservices-based)  
- **Database:** MySQL, Sequelize ORM  
- **Admin Panel:** AdminJS with custom resource configurations  
- **Authentication:** JWT-based login system
- **Features:** Progressive Web App (PWA), Responsive Design for mobile and desktop

Source code (Work in Progress): https://github.com/Thanarat-DS/E-Testing-App

## Login
ใช้ Json Web Token(JWT) ในการ Secure Login ของผู้ใช้ <br></br>
<img src="assets/login.png" height=80% width=auto></img>
## Home Page
ตัวอย่าง list ข้อสอบ แต่ละแผนกจะสอบเรื่องไม่เหมือนกัน (ในรูปเป็นข้อมูลสมมติ) <br></br>
<img src="assets/quiz_list.png"></img>
## Quiz
ตัวอย่างข้อสอบ มีการจับเวลาการทำ (ในรูปเป็นข้อมูลสมมติ) <br></br>
<img src="assets/quiz1.png"></img>
## Result
หน้าผลการสอบ เมื่อทำครบทุกข้อ <br></br>
<img src="assets/result.png"></img>
## Admin
มีหน้าหลังบ้านเพื่อให้ Admin เข้าไปจัดการและแก้ไข <br></br>
<img src="assets/home_admin.png"></img>
## Admin Edit Database
ตัวอย่างข้อมูลผู้ใช้ <br></br>
<img src="assets/user_data.png"></img>
## Custom Admin Page ในระบบสามารถสร้าง Custom Components ที่ Advanced กว่าเดิมได้
หน้า Report มุมมองแบบภาพรวม เมื่อคลิกที่รหัสข้อสอบจะสามารถ navigate พร้อม Filter เพื่อเพิ่ม/แก้ไข <br></br>
<img src="assets/custom_page1.png"></img><br></br>
หน้า Config ข้อสอบ<br></br>
<img src="assets/custom_page2.png"></img>

# 2. C# Backend Challenge
source code:https://github.com/Thanarat-DS/BackendChallenge
## 🧰 Tech Stack

- **Backend:** ASP.NET Core 8.0 (Web API)
- **Authentication:** ASP.NET Identity with JWT (JSON Web Token)
- **Database:** SQLite
- **ORM:** Entity Framework Core


## API Endpoint Summary

| Method | Endpoint       | Description                                                  | Request Body Example                                |
|--------|----------------|--------------------------------------------------------------|-----------------------------------------------------|
| POST   | `/login`       | Authenticate user and return JWT token                       | `{ "username": "xxx", "password": "xxxx" }`         |
| POST   | `/register`    | Create new user account                                      | `{ "username": "xxx", "password": "xxxx", "fullname": "xxx" }` |
| GET    | `/books`       | Get book list from ITBook API and sort by title              | –                                                   |
| POST   | `/user/like`   | Like a book and save to database                             | `{ "user_id": "xxx", "book_id": 1 }`                |

# 3. Artesian Map And Farm Analysis App

source code: https://github.com/Thanarat-DS/MapAppProject

## Overview

Interactive mapping application to visualize farmland, artesian wells, and aquifer layers. Built with React, it allows users to search farmland plots and discover nearby water resources with spatial analysis tools.

## 🧰 Tech Stack

- **Frontend:** React, Leaflet, Semantic UI
- **Data Cleaning:** Python
- **Data Visualization:** React-Leaflet (Map), Custom popups and markers

## Features

- View clustered data on an interactive map.
- Search by plot ID to find artesian wells within a 2 km radius.
- Hover over data points to:
  - See well details.
  - Identify aquifer layers.
  - Get direction and distance from selected farmland.

## Data Sources

1. **Farm Data:** Randomly generated for demonstration.
2. **Artesian Wells:** Open data from Thai Government.
3. **Aquifer Layers:** Open data from the Thai Department of Water Resources.

## UI Snapshots

**Home Page** 
 
<img src="assets/home.png" />

**Zoom-in View with Clustering**  

<img src="assets/home-zoom.png" />

**Plot Search with Nearby Wells Highlighted**  

<img src="assets/hover-artesian.png" width="70%" height="70%" />

# 4. E-Learning Website (โปรเจคตอนเรียนที่ KMITL University)

source code: https://github.com/Thanarat-DS/E-LearningWeb

## 🧰 Tech Stack

- **Frontend:** HTML, CSS
- **Backend:** PHP 
- **Database:** MySQL
- **Features:** API Payment Gateway

## Login
<img src="assets/elearn_login.png" height=80% width=50%></img>
## Register
แยก Role ระหว่างผู้สอนและผู้เรียน

<img src="assets/elearn_reg.png" height=80% width=50%></img>
## Payment Plan
<img src="assets/elearn_plan.png"></img>
## Payment Enter Credit Card
<img src="assets/elearn_pay.png"></img>
## Success Payment 
<img src="assets/elearn_success.png" width="30%" height="30%"></img>
## Home Page
<img src="assets/elearn_home.png"></img>
## Home Page (ต่อ)
<img src="assets/elearn_course.png"></img>
## Courses List
<img src="assets/elearn_s.png"></img>
## In Course
<img src="assets/elearn_incourse.png"></img>

# 5. LittleLemon API (Django Backend Challenge)

source code: https://github.com/Thanarat-DS/LittleLemon-API-Project

## Project structure and API routes

<p>
  In this project, the APIs should allow end-users to perform the following tasks
</p>

1.	The admin can assign users to the manager group
2.	You can access the manager group with an admin token
3.	The admin can add menu items 
4.	The admin can add categories
5.	Managers can log in 
6.	Managers can update the item of the day
7.	Managers can assign users to the delivery crew
8.	Managers can assign orders to the delivery crew
9.	The delivery crew can access orders assigned to them
10.	The delivery crew can update an order as delivered
11.	Customers can register
12.	Customers can log in using their username and password and get access tokens
13.	Customers can browse all categories 
14.	Customers can browse all the menu items at once
15.	Customers can browse menu items by category
16.	Customers can paginate menu items
17.	Customers can sort menu items by price
18.	Customers can add menu items to the cart
19.	Customers can access previously added items in the cart
20.	Customers can place orders
21.	Customers can browse their own orders

### User registration and token generation endpoints

You can use Djoser in your project to automatically create the following endpoints and functionalities for you.

| Endpoint                   | Role                                      | Method     | Purpose                                                                     |
| -------------------------- | ----------------------------------------- | ---------- | --------------------------------------------------------------------------- |
| **`/api/users`**           | No role required                          | **`POST`** | Creates a new user with name, email and password                            |
| **`/api/users/users/me/`** | Anyone with a valid user token            | **`GET`**  | Displays only the current user                                              |
| **`/token/login/`**        | Anyone with a valid username and password | **`POST`** | Generates access tokens that can be used in other API calls in this project |

##  Menu-items endpoints

| Endpoint                         | Role                    | Method                                           | Purpose                                                             |
| -------------------------------- | ----------------------- | ------------------------------------------------ | ------------------------------------------------------------------- |
| **`/api/menu-items`**            | Customer, delivery crew | **`GET`**                                        | Lists all menu items. Return a **`200 – Ok`** HTTP status code      |
| **`/api/menu-items`**            | Customer, delivery crew | **`POST`**, **`PUT`**, **`PATCH`**, **`DELETE`** | Denies access and returns **`403 – Unauthorized`** HTTP status code |
| **`/api/menu-items/{menuItem}`** | Customer, delivery crew | **`GET`**                                        | Lists single menu item                                              |
| **`/api/menu-items/{menuItem}`** | Customer, delivery crew | **`POST`**, **`PUT`**, **`PATCH`**, **`DELETE`** | Returns **`403 - Unauthorized`**                                    |
| **`/api/menu-items`**            | Manager                 | **`GET`**                                        | Lists all menu items                                                |
| **`/api/menu-items`**            | Manager                 | **`POST`**                                       | Creates a new menu item and returns **`201 - Created`**             |
| **`/api/menu-items/{menuItem}`** | Manager                 | **`GET`**                                        | Lists single menu item                                              |
| **`/api/menu-items/{menuItem}`** | Manager                 | **`PUT`**, **`PATCH`**                           | Updates single menu item                                            |
| **`/api/menu-items/{menuItem}`** | Manager                 | **`DELETE`**                                     | Deletes menu item                                                   |

## User group management endpoints

| Endpoint                                       | Role    | Method       | Purpose                                                                                                                                                            |
| ---------------------------------------------- | ------- | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **`/api/groups/manager/users`**                | Manager | **`GET`**    | Returns all managers                                                                                                                                               |
| **`/api/groups/manager/users`**                | Manager | **`POST`**   | Assigns the user in the payload to the manager group and returns **`201-Created`**                                                                                 |
| **`/api/groups/manager/users/{userId}`**       | Manager | **`DELETE`** | Removes this particular user from the manager group and returns **`200 – Success`** if everything is okay. If the user is not found, returns **`404 – Not found`** |
| **`/api/groups/delivery-crew/users`**          | Manager | **`GET`**    | Returns all delivery crew                                                                                                                                          |
| **`/api/groups/delivery-crew/users`**          | Manager | **`POST`**   | Assigns the user in the payload to delivery crew group and returns **`201-Created`** HTTP                                                                          |
| **`/api/groups/delivery-crew/users/{userId}`** | Manager | **`DELETE`** | Removes this user from the manager group and returns **`200 – Success`** if everything is okay. If the user is not found, returns  **`404 – Not found`**           |

## Cart management endpoints

| Endpoint                   | Role     | Method       | Purpose                                                                                         |
| -------------------------- | -------- | ------------ | ----------------------------------------------------------------------------------------------- |
| **`/api/cart/menu-items`** | Customer | **`GET`**    | Returns current items in the cart for the current user token                                    |
| **`/api/cart/menu-items`** | Customer | **`POST`**   | Adds the menu item to the cart. Sets the authenticated user as the user id for these cart items |
| **`/api/cart/menu-items`** | Customer | **`DELETE`** | Deletes all menu items created by the current user token                                        |

## Order management endpoints

| Endpoint                    | Role          | Method                 | Purpose                                                                                                                                                                                                                                                                                                                                                                   |
| --------------------------- | ------------- | ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **`/api/orders`**           | Customer      | **`GET`**              | Returns all orders with order items created by this user                                                                                                                                                                                                                                                                                                                  |
| **`/api/orders`**           | Customer      | **`POST`**             | Creates a new order item for the current user. Gets current cart items from the cart endpoints and adds those items to the order items table. Then deletes all items from the cart for this user.                                                                                                                                                                         |
| **`/api/orders/{orderId}`** | Customer      | **`GET`**              | Returns all items for this order id. If the order ID doesn’t belong to the current user, it displays an appropriate HTTP error status code.                                                                                                                                                                                                                               |
| **`/api/orders`**           | Manager       | **`GET`**              | Returns all orders with order items by all users                                                                                                                                                                                                                                                                                                                          |
| **`/api/orders/{orderId}`** | Customer      | **`PUT`**, **`PATCH`** | Updates the order. A manager can use this endpoint to set a delivery crew to this order, and also update the order status to 0 or 1. <br>If a delivery crew is assigned to this order and the **`status = 0`**, it means the order is out for delivery. <br>If a delivery crew is assigned to this order and the **`status = 1`**, it means the order has been delivered. |
| **`/api/orders/{orderId}`** | Manager       | **`DELETE`**           | Deletes this order                                                                                                                                                                                                                                                                                                                                                        |
| **`/api/orders`**           | Delivery crew | **`GET`**              | Returns all orders with order items assigned to the delivery crew                                                                                                                                                                                                                                                                                                         |
| **`/api/orders/{orderId}`** | Delivery crew | **`PATCH`**            | A delivery crew can use this endpoint to update the order status to 0 or 1. The delivery crew will not be able to update anything else in this order.                                                                                                                                                                                                                     |
