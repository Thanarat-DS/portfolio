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
