# 🎯 Event Management System - Backend API

A professional and scalable **RESTful API** built with **Node.js**, **Express**, and **MongoDB** for managing events and registrations with **JWT-based authentication** and **role-based authorization**.

This project is part of my **CodeXIntern internship**, showcasing clean architecture, secure auth, modular coding practices, and real-world backend concepts.

---

## 📌 Table of Contents

- [📌 Table of Contents](#-table-of-contents)
- [🚀 Project Overview](#-project-overview)
- [🛠️ Tech Stack](#️-tech-stack)
- [✨ Features](#-features)
- [📁 Folder Structure](#-folder-structure)
- [🔐 Environment Variables](#-environment-variables)
- [⚙️ Installation & Setup](#️-installation--setup)
- [📬 API Endpoints](#-api-endpoints)
- [📮 Postman Testing](#-postman-testing)
- [👨‍💻 Author](#-author)
- [✅ Final Notes](#-final-notes)

---

## 🚀 Project Overview

The **Event Management System** backend enables:

- 👤 User registration & login with JWT  
- 🧑‍💼 Admin-exclusive event management  
- 🙋‍♂️ User event registrations  
- 📜 Role-based access control (User/Admin)  
- ⚙️ Scalable and maintainable folder structure  

This API is built with **professional development standards** in mind and is ready for real-world deployment and integration.

---

## 🛠️ Tech Stack

| Layer        | Technology              |
|--------------|--------------------------|
| **Runtime**  | Node.js                  |
| **Framework**| Express.js               |
| **Database** | MongoDB with Mongoose    |
| **Auth**     | JSON Web Token (JWT)     |
| **Validation**| express-validator       |
| **Middleware**| Custom auth & role middleware |
| **Env Config**| dotenv                  |
| **Testing Tool**| Postman               |

---

## ✨ Features

- ✅ Secure registration and login with JWT  
- ✅ Role-based access control (Admin / User)  
- ✅ Create, read, update, delete events (Admin only)  
- ✅ Event registration for users  
- ✅ Organized MVC folder structure  
- ✅ Input validation and centralized error handling  

---

## 📁 Folder Structure

Event-Management-System/
│
├── controllers/ # Business logic (auth, events, registration)
├── middlewares/ # Auth & role-based access middleware
├── models/ # Mongoose schemas
├── routes/ # Route definitions
├── config/ # MongoDB connection setup
│
├── app.js # Main Express app configuration
├── server.js # Server start script
├── .env # Environment variables
├── package.json
└── README.md

---

## 🔐 Environment Variables

Create a `.env` file in the root directory with the following content:

PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/event_db
JWT_SECRET=yourSecretKey


---

## ⚙️ Installation & Setup

```bash
# 1. Clone the repository
git clone https://github.com/Yuvraj-Singh20/event-management-system.git


# 2. Navigate to the project directory
cd event-management-system


# 3. Install dependencies
npm install


# 4. Create a .env file and add environment variables (see above)


# 5. Start the development server
nodemon server.js
✅ Server will start on: http://localhost:5000


📬 API Endpoints
🔐 Auth Routes
Method	Route	Description	Access
POST	/api/auth/register	Register new user	Public
POST	/api/auth/login	Login existing user	Public


📅 Event Routes
Method	Route	Description	Access
POST	/api/events	Create new event	Admin
GET	/api/events	Get all events	Public
GET	/api/events/:id	Get event by ID	Public
PUT	/api/events/:id	Update existing event	Admin
DELETE	/api/events/:id	Delete an event	Admin


📝 Registration Routes
Method	Route	Description	Access
POST	/api/registrations/:eventId	Register for an event	User
GET	/api/registrations	View all registrations	Admin


📮 Postman Testing
For API testing, use Postman with these features:

🔐 Login/Register as User/Admin
📅 Create/Update/Delete events (Admin only)
📋 Register for Events (User)


🔑 Use the JWT token in the header for protected routes:

makefile
Copy
Edit
Authorization: Bearer <your_token>


You can also save two collections in Postman:
Admin Collection
User Collection


👨‍💻 Author
Yuvraj Singh
Backend Developer Intern – CodeXIntern

🔗 GitHub
💼 LinkedIn


✅ Final Notes
This is a backend-only implementation of a real-world event management system built during my internship. It reflects:

✅ Clean code and modular folder structure
✅ Secure authentication and role-based access
✅ Real-world backend development best practices
✅ Readiness for integration with a frontend UI

⭐ Feel free to fork, star, or contribute!

Thanks for visiting this project!
📦 Happy Coding!