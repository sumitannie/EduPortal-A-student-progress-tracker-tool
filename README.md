🎓 CampusAssist – Student Academics & Attendance Tracker with AI

CampusAssist is a teacher-focused academic management system designed to simplify everyday school workflows.
It enables teachers to manage student records, generate report cards, track attendance, and get academic assistance through an integrated AI chatbot.

Built with Flask and Python, the system focuses on clarity, usability, and real-world classroom needs.

✨ Key Features
📋 Student Management

- Add and store student details (Name, Roll, Class)

- Persistent storage using JSON

- View and manage all students from a single dashboard

📄 Report Card Generation

- Automatically generates school-style report cards

- Subject-wise marks and grades

- Total marks, percentage, grade, and teacher remarks

- Clean, printable layout for real classroom use

🗓 Attendance Management System

- Mark daily attendance class-wise

- Date-based attendance storage

- Persistent records across application restarts

📊 Student-wise Attendance Report

- Total working days

- Days present and absent

- Attendance percentage

- Date-wise attendance history

🤖 CampusAssist AI (Teacher Assistant)

- Built-in AI chatbot for teachers

Helps with:

- Teaching strategies

- Quiz and question generation

- Student performance guidance

- Academic planning ideas

- Supports conversation memory within a session

- Clean, bullet-point responses optimized for teachers

🔍 Smart Search & Filtering

- Search students by name

- Filter students by class

- Designed to reduce teacher cognitive load



🛠️ Tech Stack

- Frontend: HTML, CSS

- Backend: Python, Flask

- Templating: Jinja2

- AI Integration: Google Gemini API

- Session Management: Flask Sessions

- Data Storage: JSON (students.json, attendance.json)

- Environment: Python Virtual Environment

📂 Project Structure
```bash
CampusAssist/
│
├── app.py                  # Flask backend
├── students.json           # Student academic data
├── attendance.json         # Attendance records
│
├── templates/
│   ├── index.html          # Dashboard
│   ├── add_students.html  # Add student
│   ├── students.html      # Student list (search & filter)
│   ├── report.html        # Report card
│   ├── mark_attendance.html
│   ├── student_attendance.html
│   ├── ai_chat.html       # AI assistant
│   └── _topbar.html       # Reusable navigation bar
│
├── static/
│   └── styles/
│       └── style.css      # Application styling
│
├── .env                   # API keys (ignored)
├── README.md
└── venv/
```

▶️ How to Run the Project

1️⃣ Create Virtual Environment

python -m venv venv


Activate it:

Windows

venv\Scripts\activate


Mac/Linux

source venv/bin/activate

2️⃣ Install Dependencies

pip install flask python-dotenv

google-generativeai

3️⃣ Set Environment Variables

Create a .env file:

GEMINI_API_KEY=your_api_key_here

4️⃣ Run the Application
python app.py

Open in browser:

http://127.0.0.1:5000/


🧪 How It Works (Flow)

- Teacher adds student details

- System calculates grades and generates report cards

- Teacher marks daily attendance

- Attendance is stored date-wise

- Student-wise attendance reports are generated

- Teacher can consult CampusAssist AI for academic help

🎯 Use Cases

- School teachers

-  Academic record management

- Attendance tracking

- Teaching assistance via AI


🚀 Future Enhancements

- Class-wise attendance analytics

- Low-attendance alerts

- PDF export for report cards

- Teacher authentication system

- Role-based access (Admin / Teacher)

- AI-powered student performance insights