# Hospital Management System

## Project Overview
The **Hospital Management System** is a web-based application aimed at streamlining hospital operations. It offers role-based dashboards for both doctors and administrators to manage their tasks efficiently. The system automates hospital processes, reduces manual errors, and enhances workflow efficiency.

---

## Key Features

### Doctor Dashboard
- View a list of patients currently under treatment.
- Access detailed diagnostic information for individual patients.
- Perform CRUD (Create, Read, Update, Delete) operations for managing patients.
- Manage hospital medicines, including options to add or update entries.

### Admin Dashboard
- View a list of patients (non-sensitive details only).
- Manage appointments with CRUD operations.

---

## Technical Scope
- **Frontend**: Angular 14  
- **Backend**: Spring Boot  
- **Database**: MySQL8  
- **API Communication**: RESTful APIs  
- **Real-Time Notifications**: WebSocket integration  

---

## High-Level Design

### Architectural Overview
The system follows the **MVC (Model-View-Controller)** architecture for modularity, scalability, and maintainability.

### Frontend
- Built with **Angular 14**, using Angular CLI for scaffolding.
- Implements:
  - Dynamic routing via `RouterModule`.
  - Two-way data binding using `[(ngModel)]`.
  - Reactive forms powered by `FormBuilder`.
- API communication is handled through Angular services.

### Backend
- Developed using **Spring Boot**.
- **JPA/Hibernate** is used for database interaction.
- RESTful APIs support HTTP methods: `GET`, `POST`, `PUT`, `DELETE`.
- Includes WebSocket for real-time notifications.
- Ensures security with **CORS policies**.

### Database
- Built on **MySQL8**, with tables for:
  - Patients
  - Doctors
  - Medicines
  - Appointments

---

## How to Run the Application

### Prerequisites
- **Frontend**:
  - Node.js 16 or later
  - Angular CLI
- **Backend**:
  - Java 17
  - Maven
- **Database**:
  - MySQL8 or a compatible database server

### Setup Steps

#### 1. Clone the repository:
```bash
git clone git@github.com:Amarnath-Rao/Hospital_Management_Sys.git
cd Hospital_Management_Sys
```

#### 2. Frontend Setup:
Navigate to the frontend directory and install dependencies:
```bash
cd frontend
npm install
ng serve
```

#### 3. Backend Setup:
Navigate to the backend directory, build the project, and run the application:
```bash
cd backend
mvn clean install
mvn spring-boot:run
```

#### 4. Database Setup:
Import the provided database schema or create the necessary tables in MySQL as defined in the project.

#### 5. Access the Application:
- Frontend: `http://localhost:4200`
