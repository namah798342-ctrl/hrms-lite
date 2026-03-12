# HRMS Lite – Full Stack Application

A lightweight Human Resource Management System (HRMS Lite) built using **Django REST Framework (Backend)** and **React + Vite (Frontend)**.

The application allows administrators to manage employees and track daily attendance through a clean and responsive web interface.

This project was developed as part of a **Full-Stack Coding Assignment** to demonstrate practical experience with backend API design, frontend development, database integration, validation, and production deployment.

---

# Live Application

### Frontend (Vercel)

https://hrms-lite-kappa-two.vercel.app/

### Backend API (Render)

https://hrms-lite-mso6.onrender.com/

### GitHub Repository

https://github.com/namah798342-ctrl/hrms-lite

---

# Project Architecture

React Frontend → Vercel  
Django REST API → Render  
PostgreSQL Database → Neon

```
React (Vite)
     ↓
Django REST API
     ↓
Neon PostgreSQL
```

---

# Features

## Employee Management

- Add new employees  
- Unique employee ID validation  
- Email validation  
- View employee list  
- Delete employees  
- Department tracking  

---

## Attendance Management

- Mark employee attendance  
- Select date and attendance status  
- Prevent duplicate attendance entries  
- View attendance records  

---

## Dashboard

- Total employees count  
- Present employees today  
- Absent employees today  

---

## Validation & Error Handling

- Required field validation  
- Duplicate employee validation  
- Duplicate attendance validation  
- Meaningful error messages  
- Proper HTTP status codes  

---

# User Interface

- Clean and responsive layout  
- Professional dashboard cards  
- Employee data table  
- Attendance records table  
- Loading states  
- Empty states  
- Error states  

---

# Tech Stack

## Frontend

- React  
- Vite  
- Axios  
- CSS  

---

## Backend

- Python  
- Django  
- Django REST Framework  

---

## Database

- PostgreSQL (Neon)

---

## Deployment

- Vercel (Frontend)  
- Render (Backend)

---

# Project Structure

```
hrms-lite
│
├── backend
│   ├── employees
│   ├── attendance
│   ├── dashboard
│   ├── manage.py
│   └── settings.py
│
├── frontend
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── api
│   │   └── styles.css
│   ├── index.html
│   └── package.json
│
├── .gitignore
└── README.md
```

---

# API Endpoints

## Employees

GET `/api/employees/`  
Retrieve all employees

POST `/api/employees/`  
Create a new employee

DELETE `/api/employees/{id}/`  
Delete employee

---

## Attendance

GET `/api/attendance/`  
Retrieve attendance records

POST `/api/attendance/`  
Mark attendance

---

## Dashboard

GET `/api/dashboard/summary/`  
Get employee attendance summary

---

# Example Response

```json
{
  "total_employees": 5,
  "present_today": 3,
  "absent_today": 2
}
```

---

# Running the Project Locally

## Backend Setup

Navigate to backend folder

```
cd backend
```

Create virtual environment

```
python -m venv venv
```

Activate environment (Windows)

```
venv\Scripts\activate
```

Install dependencies

```
pip install -r requirements.txt
```

Run migrations

```
python manage.py migrate
```

Start server

```
python manage.py runserver
```

Backend will run on

```
http://127.0.0.1:8000
```

---

# Frontend Setup

Navigate to frontend

```
cd frontend
```

Install dependencies

```
npm install
```

Run development server

```
npm run dev
```

Frontend will run on

```
http://localhost:5173
```

---

# Deployment

## Backend Deployment

- Hosted on Render  
- Connected to Neon PostgreSQL database  
- Gunicorn used as production server  

## Frontend Deployment

- Hosted on Vercel  
- Connected to deployed backend API  

---

# Advanced Improvements

Although the assignment required a minimal system, the following improvements were considered:

- Dashboard analytics  
- Attendance summary tracking  
- Modular API structure  
- Responsive UI design  
- Proper error handling  

---

# Assumptions

- Only a single admin user manages the system  
- No authentication system required  
- Leave management and payroll are out of scope  

---

# Future Enhancements

- Authentication & role-based access  
- Employee profile editing  
- Attendance filtering by date  
- Monthly attendance reports  
- Admin dashboard analytics  
- Pagination for large datasets  
- Unit tests and API test coverage  

---

# Conclusion

HRMS Lite demonstrates a complete **full-stack workflow** including:

- Backend API design  
- Frontend UI development  
- Database integration  
- Validation and error handling  
- Production deployment  

The project focuses on delivering a **clean, stable, and functional application aligned with the requirements of the assignment**.
