# Java-Swing-Employee-Registration-and-Authentication-System-using-MySQL-JDBC-and-Maven.
A Java Swing-based Employee Registration and Authentication System that enables secure user login and employee management using MySQL and JDBC. The application supports CRUD operations, password encryption using SHA-256, and a user-friendly interface for managing employee records efficiently.
# Employee Registration and Authentication System

A Java Swing desktop application for managing employee records with secure user authentication and a MySQL database backend.

## 📌 Project Overview

The Employee Registration and Authentication System is a desktop-based application developed using Java Swing and MySQL. The system allows multiple users to register, log in securely, and manage employee records through an easy-to-use graphical interface.

The application supports CRUD operations (Create, Read, Update, Delete) on employee data and provides authentication features to ensure secure access.

---

## 🚀 Features

### User Management
- User Registration
- Secure Login Authentication
- Password Encryption using SHA-256
- Logout Functionality
- Multi-user Support

### Employee Management
- Add Employee
- View Employee Details
- Update Employee Information
- Delete Employee Records
- Search Employees

### User Interface
- Java Swing GUI
- Dashboard for Employee Management
- Employee Profile Window
- Responsive and Simple Design

---

## 🛠️ Technologies Used

- Java
- Java Swing
- JDBC
- MySQL
- Maven
- SHA-256 Password Hashing

---

## 📂 Project Structure

```
employee-system/
│
├── src/main/java/com/employeesystem/
│   ├── App.java
│   ├── dao/
│   ├── db/
│   ├── model/
│   ├── ui/
│   └── util/
│
├── database.sql
├── pom.xml
├── README.md
└── MULTI_USER_GUIDE.md
```

---

## 🗄️ Database

Database Name:

```sql
employee_system
```

The project contains two main tables:

### Users Table
- id
- username
- email
- password

### Employees Table
- emp_id
- name
- department
- email
- salary

---

## ⚙️ Installation and Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/YourUsername/employee-system.git
cd employee-system
```

### Step 2: Create Database

```bash
mysql -u root -p < database.sql
```

### Step 3: Configure Database Connection

Open:

```java
src/main/java/com/employeesystem/db/DBConnection.java
```

Update:

```java
private static final String URL = "jdbc:mysql://localhost:3306/employee_system";
private static final String USER = "root";
private static final String PASSWORD = "your_password";
```

### Step 4: Run the Application

Using Maven:

```bash
mvn compile
mvn exec:java
```

---

## 🔐 Security Features

- Passwords are encrypted using SHA-256 hashing.
- User authentication before accessing the dashboard.
- Separate user accounts with secure login credentials.

---

## 👥 Multi-User Support

- Multiple users can register and log in.
- All users share a common employee database.
- Current logged-in user is displayed on the dashboard.
- Users can log out and switch accounts.

---

## 📸 Application Modules

1. Login Screen
2. Registration Screen
3. Dashboard
4. Employee Profile Management
5. Search Employee Module

---

## 🎯 Learning Outcomes

- Java Swing GUI Development
- JDBC Connectivity
- MySQL Database Management
- Authentication Systems
- CRUD Operations
- Maven Project Structure

---

## 📌 Future Enhancements

- Role-Based Access Control (Admin/User)
- Export Employee Data to Excel/PDF
- Advanced Search Filters
- Profile Picture Support
- Email Notifications
- Cloud Database Integration

---

## 👨‍💻 Author

**Surya Kutta**
---

## 📄 License

This project is developed for educational and learning purposes.
