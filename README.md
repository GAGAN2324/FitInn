# FitSync 

A fitness tracking web application built using Java, Spring Boot, Spring Security, Spring Data JPA, and MySQL. The application provides REST APIs for user management, workout tracking, BMI calculation, weight monitoring, and dashboard analytics with a lightweight HTML/CSS/JavaScript frontend.

## Features

- JWT-based authentication with token generation and validation.
- User management through REST APIs.
- Workout tracking and workout history.
- BMI calculation and weight monitoring.
- Dashboard for fitness statistics and progress visualization.
- RESTful APIs for frontend-backend communication.
  
## Tech Stack

### Backend
- Java
- Spring Boot
- Spring Security
- Spring Data JPA
- JWT
- Maven

### Database
- MySQL

### Frontend
- HTML
- CSS
- JavaScript

  ## Backend Highlights

- Developed 18 RESTful APIs for authentication, user management, workout tracking, BMI calculation, and dashboard analytics.
- Implemented JWT token generation and validation using Spring Security.
- Integrated MySQL using Spring Data JPA for efficient CRUD operations.
- Designed the application using the Controller–Service–Repository architecture.

## Project Structure

```
microfit/
├── src/main/java/com/microfit/microfit/
│   ├── controller/   # REST controllers (Auth, User, Workout)
│   ├── model/        # JPA entities
│   ├── dto/          # Request/response DTOs
│   ├── repository/   # Spring Data repositories
│   └── security/     # JWT + Spring Security config
└── MicroFrontend/    # Static HTML/CSS/JS frontend
```

## Getting Started

### Prerequisites
- Java 17+ and Maven
- MySQL running locally

### Configure the database
Update `src/main/resources/application.properties` with your local MySQL credentials:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/microfit
spring.datasource.username=root
spring.datasource.password=your_password
```




## Architecture

Frontend (HTML/CSS/JavaScript)
        │
        ▼
Spring Boot REST APIs
        │
        ▼
Service Layer
        │
        ▼
Spring Data JPA
        │
        ▼
MySQL Database






### Run the backend
```bash
mvn spring-boot:run
```
Runs on `http://localhost:8080`.

### Run the frontend
Open `MicroFrontend/login.html` via a local static server (e.g. IntelliJ's built-in web server, or `npx serve`).


## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/auth/login | User login |
| POST | /api/auth/register | User registration |
| GET | /api/users | Get all users |
| GET | /api/users/{id} | Get user by ID |
| POST | /api/workouts | Add workout |
| GET | /api/workouts | Get workouts |
| GET | /api/dashboard | Dashboard statistics |
| GET | /api/bmi | Calculate BMI |




## Screenshots
<img width="1883" height="898" alt="image" src="https://github.com/user-attachments/assets/2ffd6ad1-fb36-49b9-a3af-907b5ee5c067" /> 
-Landing Page

<img width="1880" height="898" alt="image" src="https://github.com/user-attachments/assets/60f3ed4d-80fd-4210-bace-97314e2b4197" />
-Dashboard

<img width="1866" height="851" alt="image" src="https://github.com/user-attachments/assets/3a69df07-f046-48d0-a414-58b97f1f60f2" />
-Progress and Trends

<img width="1873" height="766" alt="image" src="https://github.com/user-attachments/assets/d32ac7ba-0606-434e-8f0c-1da5e2cc4b38" />
-Workouts


