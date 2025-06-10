# 🌱 Plant Management Backend API

A Java Spring Boot-based backend application for managing a collection of plants. It provides a set of RESTful APIs to perform CRUD operations and search functionality on plant records.

---

## 🚀 Features

- Add new plant records
- View all plants or individual plant details
- Update existing plant records
- Delete plant records
- Search plants by name or other attributes

---

## 🛠️ Tech Stack

- **Backend Framework**: Spring Boot
- **Database**: MySQL 
- **ORM**: Spring Data JPA (Hibernate)
- **Build Tool**: Maven
- **REST API**: Spring Web

---


## 📦 API Endpoints

| Method | Endpoint           | Description              |
|--------|--------------------|--------------------------|
| GET    | `/plants`          | Get all plants           |
| GET    | `/plants/{id}`     | Get plant by ID          |
| POST   | `/plants`          | Create a new plant       |
| PUT    | `/plants/{id}`     | Update a plant           |
| DELETE | `/plants/{id}`     | Delete a plant           |
| GET    | `/plants/search?`  | Search plants            |

---

## 🧪 Running the Application

### Prerequisites

- Java 17+
- Maven or Gradle
- MySQL running (or H2 for in-memory testing)

### Steps

```bash
# Clone the repository
git clone https://github.com/charan2r/plants-app.git
cd plant-manager-backend

# Add this to application.properties
spring.datasource.url=jdbc:mysql://localhost:3306/your_db_name
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update

# Build the application
./mvnw clean install

# Run the app
./mvnw spring-boot:run



