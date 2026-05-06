# 🚀 EvalPro Backend

A backend system that evaluates developer profiles using resume data and GitHub activity to generate a structured score and feedback.

---

## 🧠 Overview

EvalPro analyzes:

* 📄 Resume (skills, projects)
* 💻 GitHub activity (repositories, commits)

And produces:

* 📊 Score breakdown
* 🧾 Detailed evaluation report
* 📈 Insights for improvement

---

## 🏗️ Tech Stack

* **Java 17**
* **Spring Boot**
* **Spring Data JPA**
* **PostgreSQL**
* **Spring Security**
* **Maven**

---

## 📁 Project Structure

```
src/main/java/com/evalpro/

├── config/          # Security & app configuration
├── controller/      # REST APIs
├── service/         # Business logic
├── repository/      # Database access
├── entity/          # JPA entities
├── dto/             # Request/response models
├── scoring/         # Scoring engine (core logic)
├── util/            # Helper utilities
└── exception/       # Global error handling
```

---

## ⚙️ Setup & Run

### 1. Clone the repository

```bash
git clone https://github.com/blitzbugg/evalpro-backend.git
cd evalpro-backend
```

---

### 2. Configure Environment Variables

Set the following variables in your system:

```bash
DB_URL=jdbc:postgresql://localhost:5432/evalpro
DB_USERNAME=postgres
DB_PASSWORD=your_password
```

---

### 3. Run the application

```bash
mvn spring-boot:run
```

---

### 4. Server

```
http://localhost:8080
```

---

## 🔐 Security Note

* Passwords are stored using hashing (BCrypt)
* Sensitive configuration is managed via environment variables
* No secrets are committed to the repository

---

## 🧪 API Endpoints (Current)

### 👤 Users

#### Create User

```
POST /users
```

Request:

```json
{
  "email": "test@example.com",
  "password": "1234",
  "name": "Ananth"
}
```

---

#### Get All Users

```
GET /users
```

---

## 📌 Features (Planned)

* 📄 Resume upload & parsing
* 🔗 GitHub integration
* 🧠 Scoring engine (rule-based)
* 📊 Evaluation dashboard
* 📈 Performance tracking

---

## 🧠 Key Learning Focus

* Clean backend architecture
* Database design & normalization
* Secure API development
* Scalable scoring system design

---

## 📜 License

This project is for educational and portfolio purposes.
