# SWE306 Programming Elective II (1) TravelBlog

Spring Boot travel blog application with JSP pages, MySQL persistence, and admin/user content flows.

## Screenshots

![Home page](docs/screenshots/home.jpg)

| Destinations | Destination Detail |
| --- | --- |
| ![Destination listing](docs/screenshots/destinations.png) | ![Destination detail](docs/screenshots/destination-detail.png) |

| Packages | Booking |
| --- | --- |
| ![Travel packages](docs/screenshots/packages.png) | ![Booking form](docs/screenshots/booking.png) |

| Login |
| --- |
| ![Login page](docs/screenshots/login.png) |

## Tech Stack

- Java 21, Spring Boot 3.5
- Spring MVC, Spring Data JPA, Hibernate
- JSP/JSTL, Bootstrap
- MySQL
- Maven

## Run Locally

Create the database:

```bash
mysql -u root -p < database-init.sql
```

Configure local environment values:

```bash
export DB_URL="jdbc:mysql://localhost:3306/mytour_travel?useSSL=false&serverTimezone=UTC&allowPublicKeyRetrieval=true"
export DB_USERNAME="root"
export DB_PASSWORD="your_password"
export JWT_SECRET="change_me"
```

Start the app:

```bash
mvn spring-boot:run
```

Open `http://localhost:8080`.

## Build

```bash
mvn clean package
```
