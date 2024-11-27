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


## Screenshots
**1. Home Page of the Application:**

![Home page](https://user-images.githubusercontent.com/27400082/185591948-646bd11f-3bd0-4a44-ad5b-e0ae3add82d6.JPG)

**2. News Feeds:**

![Newsfeeds1](https://user-images.githubusercontent.com/27400082/185595973-3b879ac5-8b0c-47f9-88a7-e616b1cc4824.JPG)

**3. Doctor Login Component with Authentication:**

![Doclogin page](https://user-images.githubusercontent.com/27400082/185596164-54e22664-a9ed-47d0-a466-c7f14147324d.JPG)

**4. Doctor Dashboard Component:**

![Doctor Dashboard](https://user-images.githubusercontent.com/27400082/185596304-2fdf38c7-b56f-490d-a17d-07d48d5aeed8.JPG)

**5. Search by name feature:**

![Search by name](https://user-images.githubusercontent.com/27400082/185596480-5f990e65-bbbd-44db-988c-7445a7c6da1d.JPG)

**6. Viewing Patient Diagnostics:**

![View Patient](https://user-images.githubusercontent.com/27400082/185596650-a0456bad-82b5-423b-b2cb-a70009d28fbd.JPG)

**7. Add Patient component:**

![Add New Patient](https://user-images.githubusercontent.com/27400082/185597082-01dc90fa-079b-491b-a602-72a2c8ddc6d3.JPG)

**8. Updating Patient Details:**

![Update Patient](https://user-images.githubusercontent.com/27400082/185596743-f11c59f7-e1aa-4f99-b517-2963b53977c8.JPG)

**9. Medicine List component:**

![Medicine List](https://user-images.githubusercontent.com/27400082/185596877-dcee6f7a-5fe7-4dc5-bf5e-5e1eba7ad96b.JPG)

**10. Add Medicine component:**

![Add Medicine](https://user-images.githubusercontent.com/27400082/185597201-396c31b8-20f8-4caf-9ea9-4ba43e143daa.JPG)

**11. Admin Login component:**

![Admin Login](https://user-images.githubusercontent.com/27400082/185597341-bed9ca37-0a27-4709-9e97-06f217b65b24.JPG)

**12. Admin Dashboard component:**

![Admin Dashboard](https://user-images.githubusercontent.com/27400082/185597407-8a982dba-0724-42d7-8837-118ad7a2c704.JPG)

**13. Appointments:**

![Appointments](https://user-images.githubusercontent.com/27400082/185597534-5e430d89-4cb5-47a3-b523-058a5aebdeca.JPG)
