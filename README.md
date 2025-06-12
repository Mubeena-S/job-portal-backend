# 💼 Job Portal System

A full-stack Job Portal backend built using **Spring Boot**, **Hibernate/JPA**, **MySQL**, and **Spring Security**. This system allows users to register, login, apply for jobs, and recruiters to post and manage job listings.

---

## 🚀 Features

- 🔐 User Registration & Login (JWT Authentication)
- 👤 Role-based Access: Admin, Recruiter & Job Seeker
- 📝 Job Posting and Job Application
- 📄 Resume Upload for Applicants
- 📊 Admin Dashboard (Job/Users Statistics)
- 📬 Email Notifications (Optional Integration)

---

## 🛠️ Tech Stack

| Layer         | Technology                      |
|---------------|----------------------------------|
| Language      | Java 17                          |
| Framework     | Spring Boot, Spring Security     |
| Database      | MySQL                            |
| ORM           | Hibernate / JPA                  |
| Authentication| JWT (JSON Web Tokens)            |
| Tooling       | Maven or Gradle                  |
| Deployment    | Railway or Render (Cloud)        |

---

## 📁 Folder Structure

job-portal-backend/
├── src/
│ ├── main/
│ │ ├── java/
│ │ │ └── com.jobportal/
│ │ │ ├── controller/
│ │ │ ├── service/
│ │ │ ├── repository/
│ │ │ ├── model/
│ │ │ └── security/
│ │ └── resources/
│ │ ├── application.properties
│ │ └── static/
├── pom.xml
└── README.md


---

## 🔧 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/Mubeena-S/job-portal-backend.git
cd job-portal-backend

**### 2. Configure MySQL Database

Create a MySQL database named `job_portal` and update your `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/job_portal
spring.datasource.username=your_username
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect

spring.security.user.name=admin
spring.security.user.password=admin

### 3. Build the project

```bash
mvn clean install

### 4. Run the application

```bash
mvn spring-boot:run
Server will start at: http://localhost:8080

##📬 Sample API Endpoints

| Method | Endpoint              | Description                 |
|--------|-----------------------|-----------------------------|
| POST   | `/api/auth/register`  | Register new user           |
| POST   | `/api/auth/login`     | Login and receive JWT token |
| GET    | `/api/jobs`           | Get all job listings        |
| POST   | `/api/jobs`           | Add new job (recruiter)     |
| POST   | `/api/jobs/{id}/apply`| Apply to a job              |

> 🔐 Secure endpoints require Bearer token in Authorization header.

## 📦 Future Enhancements

- 📧 Email verification during signup  
- 📁 Resume upload via file storage  
- 📊 Admin dashboard frontend (React)  
- 📍 Filter & Search for jobs  
- 📱 Mobile responsiveness (via frontend)

## 🙋‍♀️ Author

**Mubeena Savalagi**  
[LinkedIn](https://www.linkedin.com/in/mubeena-savalagi-0490a91b7)  
📧 savalagimubeena@gmail.com

---

## 🌟 Support

If you found this project useful, please ⭐ star the repo and share!

