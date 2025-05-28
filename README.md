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
