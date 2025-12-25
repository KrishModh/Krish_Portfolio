
# 🌐 Full-Stack Portfolio Website with Admin Panel

A modern, responsive, and dynamic portfolio web application built with React (Vite), Flask (Python), and Oracle Database.  
Includes a secure **Admin Panel** to upload Projects, Certificates, and manage Contact Messages — all stored in database and displayed dynamically on user portfolio.



---

## ✨ Features

### 🧑‍💻 User Side (Portfolio)
✔️ Modern UI with Dark/Light mode  
✔️ Dynamic Projects & Certificates from Database  
✔️ Contact form with backend storage  
✔️ Resume Download  
✔️ Social Links (GitHub, LinkedIn)  
✔️ Fully responsive (Mobile + Desktop)

### 🔐 Admin Panel
✔️ Login authentication (JWT)  
✔️ Upload Projects & Certificates  
✔️ Manage Messages (Mark as Read/Unread)  
✔️ Message Read/Unread Counter  

---

## 🛠 Tech Stack

| Layer | Technologies |
|-------|--------------|
| Frontend | React (Vite), CSS, React Router |
| Admin Frontend | React, JWT Auth |
| Backend API | Flask, Flask-CORS |
| Database | Oracle SQL |
| Hosting | Ngrok (Temp), Vercel & Render (Future) |

---

## 📂 Folder Structure

```
portfolio-fullstack/
│
├── admin-frontend/       
├── user-frontend/        
├── backend-api/          
│    ├── app/
│    │   ├── routes/      
│    │   ├── models/      
│    │   └── uploads/     
│
├── .gitignore
├── README.md
└── commands of sql.txt
```

---

## 🔗 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/projects | Fetch all portfolio projects |
| POST | /api/admin/projects | Upload new project |
| GET | /api/certificates | Fetch certificates |
| POST | /api/admin/certificates | Upload certificate |
| GET | /api/messages | Fetch messages |
| POST | /contact | Submit portfolio message |

---

## 🖼 Screenshots

## 🧑‍💻 User Side

| Home Page | About Page |
|-----------|---------------|
|<img width="2560" height="1440" alt="Screenshot (454)" src="https://github.com/user-attachments/assets/6a541c82-f105-4c0d-8039-4b123b3340bb" /> | <img width="2560" height="1440" alt="Screenshot (455)" src="https://github.com/user-attachments/assets/31bbb9a3-6aa4-4b21-b7ce-500fb7ed9eca" /> |

| Certificates | Projects Page |
|--------------|--------------|
| <img width="2560" height="1440" alt="Screenshot (456)" src="https://github.com/user-attachments/assets/1a882b7d-5919-4883-a5ab-0577239f493b" /> | <img width="2560" height="1440" alt="Screenshot (457)" src="https://github.com/user-attachments/assets/bc02af46-3565-4ab1-9082-d188e577b8f8" /> |

| Contact Page |
|--------------|
| <img width="2560" height="1440" alt="Screenshot (458)" src="https://github.com/user-attachments/assets/4709b52f-6c3b-4ccb-96de-a5cc57e71da7" /> |

## 🔐 Admin Side
| Upload Projects Page | Upload Certificate Page | Messages Page |
|--------------|--------------|--------------|
| <img width="2560" height="1440" alt="Screenshot (460)" src="https://github.com/user-attachments/assets/0de1338d-e023-4228-85e6-d92e970b6989" /> | <img width="2560" height="1440" alt="Screenshot (461)" src="https://github.com/user-attachments/assets/205e146a-f586-4a3a-b6ac-592bbcc7d499" /> | <img width="2560" height="1440" alt="Screenshot (463)" src="https://github.com/user-attachments/assets/d58592e4-5d70-49d9-b1f4-782e889a0793" /> |
---

## 📄 Database Tables (Oracle SQL)

```sql
CREATE TABLE projects (
  id NUMBER PRIMARY KEY,
  title VARCHAR2(200),
  description CLOB,
  tech_stack VARCHAR2(500),
  image_url VARCHAR2(300),
  github_link VARCHAR2(200),
  demo_link VARCHAR2(200)
);

CREATE TABLE certificates (
  id NUMBER PRIMARY KEY,
  title VARCHAR2(200),
  issuer VARCHAR2(200),
  year VARCHAR2(20),
  image_url VARCHAR2(300),
  cert_link VARCHAR2(200)
);

CREATE TABLE messages (
  id NUMBER PRIMARY KEY,
  name VARCHAR2(100),
  email VARCHAR2(100),
  message CLOB,
  created_at TIMESTAMP,
  is_read NUMBER(1) DEFAULT 0
);
```

---

## 📞 Contact

👨‍💻 Developed by: **{{ Krish Modh }}**  
🔗 LinkedIn: _https://www.linkedin.com/in/krish-modh-b38447300?utm_source=share_via&utm_content=profile&utm_medium=member_android_  
💻 GitHub: _https://github.com/KrishModh_  
📧 Email: _rmodh4@gmail.com_  

⭐ If you like this project, consider giving it a star!
