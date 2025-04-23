# 📚 Quiz Master

Quiz Master is a full-stack web application designed to manage and take quizzes in an educational setting. It allows users to register, log in, and attempt scheduled quizzes, while admins can perform full CRUD operations on subjects, chapters, quizzes, and questions.

## 🚀 Features

### 👨‍🎓 User
- Register and log in securely
- View available quizzes based on scheduled dates
- Attempt quizzes and receive scores instantly
- Track quiz history and performance statistics
- Search past attempts and quizzes

### 🧑‍💼 Admin
- Built-in admin user (username: admin, password: admin123)
- Create, Read, Update, Delete:
  - Subjects
  - Chapters (linked to subjects)
  - Quizzes (linked to chapters)
  - Questions (linked to quizzes)
- View and manage registered users
- Analyze user performance through quiz attempts and scores

## 🗂 Database Schema

- User: Stores user details and admin status
- Subject: Each subject can contain multiple chapters
- Chapter: Linked to subjects and can contain multiple quizzes
- Quiz_table: Stores quiz details like name, duration, date, etc.
- Question_Table: Contains all questions, options, correct answers, and marks
- Quiz_Attempt_Table: Tracks user answers and their correctness
- Score_Table: Stores user scores, time taken, and total attempts

## 🛠️ Tech Stack

- Backend: Flask, Flask-SQLAlchemy
- Frontend: HTML, Jinja2, Bootstrap
- Database: SQLite
- Data Visualization: Chart.js

## 🏗 Project Structure

```
QUIZ_MASTER/
├── app.py                      # Application entry point
├── application/
│   ├── config.py               # App configuration
│   ├── database.py             # DB setup and initialization
│   ├── models.py               # Database schema definitions
├── controllers/
│   ├── admin_controllers/      # Admin functionality
│   ├── user_controllers/       # User functionality
├── templates/
│   ├── admin_templates/        # Admin HTML templates
│   ├── user_templates/         # User HTML templates
│   ├── login.html, logout.html # Common auth templates
├── static/                     # CSS, images, and other assets
```


## 🧪 How to Run

1. Clone the repo:
   git clone https://github.com/adityaNarthi/Quiz_Master.git
   cd Quiz_Master

2. Create a virtual environment & activate it:
   python -m venv venv
   venv\Scripts\activate  # On Windows

3. Install dependencies:
   pip install -r requirements.txt

4. Run the app:
   python app.py

App will be available at http://localhost:5000

## 👤 Author

Aditya Basavaraj Narthi  
3rd Year ECE Student | IIT Madras
📧 anarthi2004@gmail.com
📧 24dp3000019@ds.study.iitm.ac.in
