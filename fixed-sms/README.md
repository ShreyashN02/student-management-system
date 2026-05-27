# 🎓 Student Management System

A full-stack web application built with **Spring Boot**, **Thymeleaf**, and **MySQL** that allows you to manage student records with full CRUD operations.

---

## 🚀 Features

- ✅ View all students in a clean table layout
- ✅ Add a new student
- ✅ Update existing student details
- ✅ Delete a student
- ✅ Responsive UI using Bootstrap 4

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Java 17+ | Backend programming language |
| Spring Boot 3.0.4 | Application framework |
| Spring Data JPA | Database interaction |
| Hibernate | ORM (Object Relational Mapping) |
| MySQL | Relational database |
| Thymeleaf | Server-side HTML templating |
| Bootstrap 4 | Frontend styling |
| Maven | Build and dependency management |

---

## 📁 Project Structure

```
student-management-system/
├── src/
│   ├── main/
│   │   ├── java/net/javaguides/sms/
│   │   │   ├── controller/
│   │   │   │   └── StudentController.java    # Handles HTTP requests
│   │   │   ├── entity/
│   │   │   │   └── Student.java              # Student data model
│   │   │   ├── repository/
│   │   │   │   └── StudentRepository.java    # Database operations
│   │   │   ├── service/
│   │   │   │   ├── StudentService.java       # Service interface
│   │   │   │   └── impl/
│   │   │   │       └── StudentServiceImpl.java  # Service logic
│   │   │   └── StudentManagementSystemApplication.java
│   │   └── resources/
│   │       ├── templates/
│   │       │   ├── students.html             # List all students
│   │       │   ├── create_student.html       # Add student form
│   │       │   └── edit_student.html         # Edit student form
│   │       └── application.properties        # App configuration
└── pom.xml                                   # Maven dependencies
```

---

## ⚙️ How to Run This Project

### Prerequisites
Make sure you have the following installed:
- [Java JDK 17+](https://www.oracle.com/java/technologies/downloads/)
- [MySQL](https://dev.mysql.com/downloads/)
- [Eclipse IDE](https://www.eclipse.org/downloads/) or [IntelliJ IDEA](https://www.jetbrains.com/idea/)
- [Maven](https://maven.apache.org/) (comes with Eclipse/IntelliJ)

---

### Step 1 — Create MySQL Database

Open MySQL and run:
```sql
CREATE DATABASE sms;
```

---

### Step 2 — Configure Database

Open `src/main/resources/application.properties` and update your MySQL credentials:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/sms?useSSL=false&serverTimezone=UTC&allowPublicKeyRetrieval=true
spring.datasource.username=root
spring.datasource.password=your_password_here
```

---

### Step 3 — Run the Application

**Option A — Using Eclipse:**
1. Import project: File → Import → Existing Maven Projects
2. Right-click project → Run As → Spring Boot App

**Option B — Using Terminal:**
```bash
cd student-management-system
./mvnw spring-boot:run
```

---

### Step 4 — Open in Browser

```
http://localhost:9999/students
```

---



## 🗄️ Database Table

The app automatically creates this table in MySQL:

```sql
CREATE TABLE students (
    id BIGINT AUTO_INCREMENT PRIMARY KEY,
    first_name VARCHAR(255) NOT NULL,
    last_name VARCHAR(255),
    email VARCHAR(255)
);
```

---

## 👤 Author

**Shreyash Narad **  
Java Developer | Internship Applicant  
📧 shreyashnarad123@gmail.com  
🐙 [GitHub Profile](https://github.com/ShreyashN02)


