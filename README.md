# 🚗 Car Rental Management System

A full-stack car rental marketplace that connects **renters** and **car owners**. Renters can search, view and book cars, while owners can list and manage their vehicles and track rentals and orders.

Built with **React.js**, **Spring Boot** and **MySQL**.

---

## ✨ Features

### For Renters
- Browse cars with category-based navigation
- Advanced search with multi-filter support: make, model, category, year range and price range
- Detailed listing pages with image galleries, specs (mileage, transmission, fuel type, body type, seating), pricing and ratings
- Book cars and manage orders and rentals
- Profile management

### For Car Owners
- Add and manage car listings
- Track rented cars
- View and manage incoming orders

### General
- Role-based dashboards for renters and owners
- Responsive UI that works on desktop and mobile
- RESTful API backend

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | React.js, JavaScript, HTML5, CSS3, Vite |
| Backend | Java, Spring Boot, REST APIs |
| Database | MySQL |
| Build Tools | Maven, npm |
| Deployment | Docker, Docker Compose |

---

## 📁 Project Structure

```
Car_Rental_Spring-boot_React/
├── React/              # Frontend (React + Vite)
│   ├── public/         # Static assets and images
│   ├── src/            # Components, pages, styles
│   └── package.json
├── Spring Boot/        # Backend (Spring Boot + Maven)
│   ├── src/            # Controllers, services, repositories, entities
│   ├── pom.xml
│   ├── Dockerfile
│   └── docker-compose.yml
├── LICENSE
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher) and npm
- Java JDK 17 or higher
- Maven (or use the included `mvnw` wrapper)
- MySQL Server

### 1. Clone the repository
```bash
git clone https://github.com/Sachinjc/your-repo-name.git
cd your-repo-name
```

### 2. Set up the database
Create a MySQL database:
```sql
CREATE DATABASE car_rental;
```

### 3. Run the backend
```bash
cd "Spring Boot"
```
Open `src/main/resources/application.properties` and set your own database details:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/car_rental
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```
Then start the server:
```bash
./mvnw spring-boot:run
```
On Windows use `mvnw.cmd spring-boot:run`. The API runs at `http://localhost:8080`.

### 4. Run the frontend
Open a new terminal:
```bash
cd React
npm install
npm run dev
```
The app runs at `http://localhost:5173`.

### Run with Docker (optional)
```bash
cd "Spring Boot"
docker-compose up --build
```

---

## 📸 Screenshots

> Add your screenshots here (home page, search results, listing details, renter dashboard, owner dashboard).

| Home Page | Car Listing |
|-----------|-------------|
| ![Home](screenshots/home.png) | ![Listing](screenshots/listing.png) |

| Renter Dashboard | Owner Dashboard |
|------------------|-----------------|
| ![Renter](screenshots/renter-dashboard.png) | ![Owner](screenshots/owner-dashboard.png) |

---

## 🔮 Future Improvements

- Online payment integration
- Email and SMS booking notifications
- Reviews and rating management
- Admin dashboard
- Availability calendar for each car

---

## 👤 Author

**Sachin Kumar**
B.Tech Computer Engineering, J.C. Bose University of Science & Technology, YMCA, Faridabad

- GitHub: [Sachinjc](https://github.com/Sachinjc)
- LinkedIn: [sachinkumar121d](https://www.linkedin.com/in/sachinkumar121d/)

---

## 📄 License

This project is licensed under the terms of the [LICENSE](LICENSE) file.
