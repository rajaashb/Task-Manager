## 📝 Task Manager

A simple and elegant web-based Task Manager built with Flask and SQLite, designed to help users create, update, and manage daily tasks. It supports light/dark mode toggling and offers a sleek, responsive UI.

--------

## 📁 Project Structure

TaskManager/

├── static/

│   └── style.css

├── templates/

│   └── index.html

├── venv/

│   └── ... (Virtual environment files)

├── app.py

├── database.db

└── README.md

--------

## 🚀 Features

- ✅ Add tasks with title and optional description

- 🔄 Update tasks by toggling their completion status

- 🗑️ Delete tasks with one click

- 🌙 Dark/Light mode toggle with local storage preference

- 🗂️ SQLite backend for persistent data storage

- 💅 Responsive and clean UI styled with CSS

--------

## 🔧 Setup Instructions

1. **Clone the Repository:** git clone https://github.com/rajaashb/Task-Manager.git

2. **Navigate to the project directory:** cd project_path

3. **Set Up a Virtual Environment:** python -m venv venv
   
   source venv/bin/activate   # On Windows: venv\Scripts\activate

4. **Install Dependencies:** pip install flask

5. **Run the Application:** python app.py

By default, the app will be available at http://127.0.0.1:5000

--------

## 💻 Usage

- Enter a task title (required) and an optional description in the form.

- Click Add Task to store it.

- Use the checkbox to mark the task as completed or not.

- Click Delete to remove a task.

- Use the Theme toggle at the top right to switch between light and dark mode. Your preference will be saved locally.

--------

## 🛠️ Technologies Used

- Frontend: HTML, CSS, JavaScript

- Backend: Python, Flask

- Database: SQLite

--------

## ⚙️ Code Overview

**app.py**

- Main Flask application.

- Routes:
  
  / – Show all tasks
  
  /add – Add new task
  
  /update/<id>/<status> – Toggle task completion
  
  /delete/<id> – Delete task

**templates/index.html**

- HTML structure using Jinja2 for dynamic content.

- Includes dark/light mode toggle script.

**static/style.css**

- Full styling for light and dark modes.

- Responsive layout with theme support and form styling.

**database.db**

- SQLite database used to store tasks persistently.

--------

## 📌 Notes

- Ensure database.db is created automatically on the first run via create_table() in app.py.

- All data is stored locally — no cloud support or user accounts.
