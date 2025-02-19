# Task Manager App

##  Project Overview
The **Task Manager App** is a simple web application that allows users to manage their tasks efficiently. It includes features such as creating, updating, deleting, and organizing tasks based on priority and completion status.

##  Features
- Create, read, update, and delete tasks.
- Set a priority level for each task (High, Medium, Low).
- Mark tasks as **"Completed"** or **"Pending"**.
- Display tasks with sorting and filtering options.

##  Tech Stack
### **Frontend:**
- **React.js** or **Next.js** for the UI.
- **Tailwind CSS** for responsive and minimal styling.

### **Backend:**
- **Node.js** with **Express.js** for the server.
- **MongoDB** for storing tasks.

### **API Routes:**
- `GET /tasks` - Retrieve all tasks.
- `POST /tasks` - Add a new task.
- `PUT /tasks/:id` - Update a task.
- `DELETE /tasks/:id` - Delete a task.

##  Other Features
- JWT-based authentication with login/signup.
- Deployment on **Vercel**.

##  Project Setup

### ** 1️. Clone the Repository**
```bash
git https://github.com/Trtheo/IMC_Task_Manager.git

cd IMC_Task_Manager

Install Dependencies

# Install frontend dependencies
cd frontend
npm install

# Install backend dependencies
cd ../server
npm install

Run the Application
# Start the backend server
cd backend
npm nodemon server.js

# Start the frontend
cd  frontend
npm npm start


