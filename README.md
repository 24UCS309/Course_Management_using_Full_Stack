# 📚 Course Management System

## 📌 Overview

This is a **web-based Course Management System (CMS)** built using:

* React.js (Frontend)
* Node.js & Express.js (Backend)
* MySQL (Database)

The system helps manage:

* Students
* Instructors
* Courses
* Assignments

It provides a simple and efficient way to handle academic data and course-related activities.

---

## 🚀 Features

* 👩‍🎓 Student Dashboard (view courses & assignments)
* 👨‍🏫 Instructor Dashboard (manage courses)
* 📚 Add & manage courses
* 📝 Upload and track assignments
* 📋 View enrolled students
* 📊 Basic progress tracking

---

## 🛠️ Technologies Used

* **Frontend:**

  * React.js
  * HTML, CSS, JavaScript

* **Backend:**

  * Node.js
  * Express.js

* **Database:**

  * MySQL

---

## 🗄️ Database Design (MySQL)

### Tables:

* **Users**

  * id, name, email, password, role

* **Courses**

  * course_id, title, description, instructor_id

* **Enrollments**

  * id, student_id, course_id

* **Assignments**

  * assignment_id, course_id, title, due_date

* **Submissions**

  * submission_id, assignment_id, student_id, file

---

## 📂 Project Structure

```id="projstruct"
CMS_PROJECT/
│── frontend/
│   ├── src/
│   ├── components/
│   └── pages/
│
│── backend/
│   ├── routes/
│   ├── controllers/
│   ├── config/
│   └── server.js
│
│── database/
│   └── schema.sql
│
│── README.md
```

---

## ⚙️ How to Run

### 🔧 Backend Setup

```bash id="cmd1"
cd backend
npm install
npm start
```

---

### 💻 Frontend Setup

```bash id="cmd2"
cd frontend
npm install
npm start
```

---

## 🗄️ MySQL Setup

1. Install MySQL server
2. Create database:

```sql id="sql1"
CREATE DATABASE cms_db;
```

3. Import schema:

```bash id="cmd3"
mysql -u root -p cms_db < database/schema.sql
```

---

## 🔑 Environment Variables

Create a `.env` file in backend:

```id="env"
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=cms_db
PORT=5000
```

---

## 🧪 Sample Flow

```id="flow"
1. User registers / logs in
2. Instructor creates course
3. Students enroll in course
4. Instructor uploads assignments
5. Students submit assignments
```

---

## ⚠️ Important Notes

* Ensure MySQL server is running
* Do not share database credentials
* Keep `.env` file secure

---

## 📈 Future Improvements

* 🔐 JWT Authentication system
* ✏️ Update/Delete features
* 🔎 Search courses
* 📱 Responsive UI

---

## 👩‍💻 Author

**Your Name**

---

⭐ If you like this project, give it a star on GitHub!
