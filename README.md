<div align="center">

# 🚗 RideShare

### **Car Pooling & Ride Sharing Platform**

**Share the ride. Split the cost. Make every journey smarter.**

<p>
  <img src="assets/rideshare-car.gif" alt="RideShare animated car" width="900">
</p>

<p>
  <img src="https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=openjdk&logoColor=white">
  <img src="https://img.shields.io/badge/Spring%20Boot-3.3.4-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
  <img src="https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
  <img src="https://img.shields.io/badge/JSP-Servlets-6A1B9A?style=for-the-badge">
  <img src="https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white">
</p>

</div>

---

## 🌟 About the Project

**RideShare** is a web-based car pooling and ride sharing platform developed to make daily commuting **simpler, more affordable, and more organized**.

The platform connects **drivers and passengers** travelling on similar routes. Drivers can offer rides and manage vehicles, while passengers can discover rides, reserve seats, manage bookings, rate completed rides, receive notifications, and report issues.

An **Admin Panel** provides tools for user management and issue resolution.

> 💡 **Goal:** Build one complete platform where ride discovery, booking, ride management, feedback, notifications, and administration work together.

---

## ⚡ What Can You Do?

<table>
<tr>
<td width="33%" valign="top">

### 👤 Passenger

- 🔐 Register & login
- 🔎 Find available rides
- 🚘 View ride details
- 🎫 Book seats
- 📋 Manage bookings
- ❌ Cancel bookings
- ⭐ Rate rides
- 🔔 Check notifications
- 🚨 Report issues
- 👤 Manage profile

</td>
<td width="33%" valign="top">

### 🚗 Driver

- 🔐 Secure login
- 🚙 Manage vehicles
- ➕ Offer rides
- 🗺️ Manage offered rides
- 👥 Manage ride bookings
- ✅ Complete/cancel rides
- 🔔 Receive notifications
- 👤 Manage profile

</td>
<td width="33%" valign="top">

### 🛡️ Admin

- 📊 Admin dashboard
- 👥 Manage users
- 🚫 Suspend users
- 🔄 Reactivate users
- 🚨 Review reports
- ✅ Resolve issues
- 📈 Monitor platform activity

</td>
</tr>
</table>

---

## 🎨 Highlights

| 🚀 Feature | 💬 Description |
|---|---|
| 🔐 Authentication | Secure login and registration with BCrypt password hashing |
| 🎭 Role-Based Access | Separate workflows for Passenger, Driver and Admin |
| 🚘 Ride Management | Drivers can create and manage available rides |
| 🎫 Booking System | Passengers can reserve and manage seats |
| 🚙 Vehicle Management | Drivers can add and manage their vehicles |
| ⭐ Ratings | Users can rate completed rides |
| 🔔 Notifications | Important ride and booking updates |
| 🚨 Issue Reporting | Users can report problems for admin review |
| 🗄️ Database Validation | Unique keys, checks and relational constraints |
| 📱 Responsive UI | CSS and JavaScript for an interactive interface |

---

## 🧩 Technology Stack

<div align="center">

| Layer | Technology |
|:---:|:---|
| 💻 Language | **Java 21** |
| ⚙️ Backend | **Spring Boot 3.3.4** |
| 🌐 Web | **Spring MVC** |
| 🖥️ View | **JSP + JSTL** |
| 🔌 Database Access | **JDBC / Spring JDBC** |
| 🗃️ Database | **MySQL 8** |
| 🔒 Security | **BCrypt** |
| 📦 Build | **Maven** |
| 🧰 IDE | **Eclipse** |
| 🎨 Frontend | **HTML, CSS, JavaScript** |

</div>

---

## 🏗️ Architecture

```text
                    ┌───────────────────────┐
                    │       🌐 Browser      │
                    └───────────┬───────────┘
                                │
                                ▼
                 ┌──────────────────────────┐
                 │ JSP / HTML / CSS / JS    │
                 └────────────┬─────────────┘
                              │
                              ▼
                 ┌──────────────────────────┐
                 │   Spring MVC Controllers │
                 └────────────┬─────────────┘
                              │
                              ▼
                 ┌──────────────────────────┐
                 │      Service Layer       │
                 └────────────┬─────────────┘
                              │
                              ▼
                 ┌──────────────────────────┐
                 │        DAO Layer         │
                 └────────────┬─────────────┘
                              │
                              ▼
                 ┌──────────────────────────┐
                 │       JDBC / MySQL       │
                 └──────────────────────────┘
```

The layered architecture keeps **presentation, business logic, and database operations separated**, making the application easier to maintain and extend.

---

## 📁 Project Structure

```text
RideShare/
│
├── 📂 database/
│   ├── schema.sql
│   ├── sample-data.sql
│   ├── constraints.sql
│   ├── queries.sql
│   └── reset-demo.sql
│
├── 📂 src/main/java/com/carpooling/
│   ├── 📂 controller/
│   │   ├── AdminController.java
│   │   ├── AuthController.java
│   │   ├── BookingController.java
│   │   ├── RatingController.java
│   │   ├── RideController.java
│   │   ├── UserController.java
│   │   └── VehicleController.java
│   │
│   ├── 📂 dao/
│   ├── 📂 model/
│   └── 📂 service/
│
├── 📂 src/main/resources/
│   ├── application.properties
│   └── 📂 static/
│       ├── 📂 css/
│       ├── 📂 js/
│       └── 📂 images/
│
├── 📂 src/main/webapp/WEB-INF/views/
│   ├── 📂 admin/
│   └── *.jsp
│
├── 📄 pom.xml
├── 📄 setup-database.bat
├── 📄 run-project.bat
└── 📄 README.md
```

---

## 🔄 How RideShare Works

### 👤 Passenger Journey

```text
🏠 Home
   ↓
🔐 Register / Login
   ↓
🔎 Find Ride
   ↓
🚘 Ride Details
   ↓
🎫 Book Ride
   ↓
✅ Booking Confirmation
   ↓
📋 My Bookings
   ↓
⭐ Rate / ❌ Cancel
   ↓
🔔 Notifications
   ↓
🚨 Report Issue
```

### 🚗 Driver Journey

```text
🔐 Login
   ↓
📊 Dashboard
   ↓
🚙 My Vehicles
   ↓
➕ Offer Ride
   ↓
🗺️ Ride Management
   ↓
👥 Bookings
   ↓
✅ Complete / ❌ Cancel
   ↓
🔔 Notifications
```

### 🛡️ Admin Journey

```text
🔐 Admin Login
      ↓
📊 Admin Dashboard
      ↓
👥 User Management
      ↓
🚫 Suspend / 🔄 Reactivate
      ↓
🚨 Reports
      ↓
✅ Resolve Issues
```

---

## 🔒 Security & Validation

RideShare includes application-level and database-level validation such as:

- 🔐 BCrypt password hashing
- 🎭 Role-based application flows
- 👤 User authentication and sessions
- 📧 Unique email validation
- 📱 Unique phone validation
- 🚙 Unique vehicle number validation
- 💺 Ride seat validation
- 💰 Ride cost validation
- 📝 Input validation
- 🎫 Booking validation
- 🚨 Report management

---

## 🗄️ Database

The application uses **MySQL** with core entities including:

```text
┌──────────────┐
│    users     │
└──────┬───────┘
       │
       ├──────────────► vehicles
       │
       └──────────────► rides
                          │
                          ├────────► bookings
                          ├────────► ratings
                          ├────────► notifications
                          └────────► reports
```

Database scripts are available inside the `database/` directory.

---

## 🚀 Getting Started

### 1️⃣ Requirements

Install:

- **JDK 21**
- **MySQL 8**
- **Eclipse IDE**
- **Maven**

### 2️⃣ Clone

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd RideShare
```

### 3️⃣ Create Database

Start MySQL and execute the supplied database scripts.

For the demo database:

```sql
SOURCE database/reset-demo.sql;
```

You can also execute the SQL files through MySQL Workbench.

### 4️⃣ Configure Database

The application uses:

```text
Database : carpooling_db
Host     : localhost
Port     : 3306
Username : root
```

The password is read from:

```text
DB_PASSWORD
```

Example:

```text
DB_PASSWORD=YourMySQLPassword
```

> ⚠️ Do not commit real database passwords or secrets to GitHub.

### 5️⃣ Import into Eclipse

```text
Eclipse
 → File
 → Import
 → Maven
 → Existing Maven Projects
 → Select RideShare
 → Finish
```

Make sure the project uses **JDK 21**.

### 6️⃣ Run

Run:

```text
CarPoolingApplication.java
```

Then open:

```text
http://localhost:8080/
```

---

## 🧪 Demo Accounts

For the seeded demo database:

| Role | Email |
|:---:|---|
| 🛡️ Admin | `admin@carpooling.com` |
| 🚗 Driver | `rahul.driver@example.com` |
| 🚗 Driver | `ananya.driver@example.com` |
| 👤 Passenger | `shashank@example.com` |
| 👤 Passenger | `priya@example.com` |

**Demo password:**

```text
password123
```

> ⚠️ Demo credentials are for local/academic testing only.

---

## 🎯 Project Objective

RideShare aims to provide a convenient digital platform for people travelling on similar routes.

### Core objectives

- 🚗 Encourage shared transportation
- 💰 Reduce commuting costs
- 🌱 Improve vehicle utilization
- 🔎 Simplify ride discovery
- 🎫 Make booking management easier
- ⭐ Enable user feedback
- 🔔 Keep users informed through notifications
- 🛡️ Provide administrative control

---

## 🧪 Testing & Demonstration

For an academic/project demonstration:

```text
1. Start MySQL
        ↓
2. Prepare database
        ↓
3. Run Spring Boot application
        ↓
4. Passenger registration/login
        ↓
5. Search & book a ride
        ↓
6. Driver creates vehicle
        ↓
7. Driver offers a ride
        ↓
8. Manage booking / rating
        ↓
9. Show notifications
        ↓
10. Submit a report
        ↓
11. Login as Admin
        ↓
12. Manage users & resolve reports
```

---

## 🔮 Future Enhancements

| Feature | Idea |
|---|---|
| 📍 Live Tracking | Real-time GPS ride tracking |
| 🗺️ Smart Routes | Map-based route optimization |
| 💳 Payments | Online payment and expense splitting |
| 💬 Chat | Real-time driver/passenger communication |
| 📱 Mobile App | Android/iOS companion application |
| 🤖 AI Recommendations | Intelligent ride matching |
| 🔔 Push Notifications | Real-time mobile alerts |
| 📊 Analytics | Advanced admin analytics dashboard |

---



---

## 💻 Built With

```text
Java 21
   +
Spring Boot
   +
Spring MVC
   +
JSP / JSTL
   +
JDBC
   +
MySQL
   +
HTML / CSS / JavaScript
   =
🚗 RideShare
```

---

<div align="center">

## ⭐ Like the Project?

If you find **RideShare** useful or interesting, consider giving this repository a ⭐

### 🚗 Share the ride.  
### 💰 Split the cost.  
### 🌱 Travel smarter.

**Made with ☕ Java and lots of debugging.**

</div>
