# 🏨 Hotel Booking System (Java + JDBC + PostgreSQL)

A console-based Java project that allows a hotel receptionist to manage bookings in a PostgreSQL database. Built using core Java, JDBC, and PostgreSQL.

---

## 💡 Project Overview

This Hotel Booking System helps receptionists:
- Add new reservations
- View all current bookings
- Fetch room number using guest details
- Update existing reservations
- Delete bookings if needed

Perfect for understanding how to connect Java to a relational database using JDBC.

---

## 🔧 Tech Stack

- **Java** (JDK 17+)
- **JDBC** (Java Database Connectivity)
- **PostgreSQL** (Database)
- IDE: IntelliJ IDEA

---

## 📋 Features

| # | Feature                | Description                                           |
|---|------------------------|-------------------------------------------------------|
| 1 | New Reservation        | Insert guest name, room number, contact              |
| 2 | View Reservations      | Display all records from the database                |
| 3 | Get Room Number        | Fetch room number by guest name + reservation ID     |
| 4 | Update Reservation     | Modify guest name, room number, contact info         |
| 5 | Delete Reservation     | Delete a reservation by ID                           |

---

## 🛠️ How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/hotel-reservation-system.git

2. Set up your PostgreSQL DB:
   ```sql
   CREATE DATABASE hotel_db;
   CREATE TABLE reservations (
    reservation_id SERIAL PRIMARY KEY,
    guest_name VARCHAR(100),
    room_number INT,
    contact_number VARCHAR(20),
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );

3. Update DB credentials in the code:
   ```java
   private static final String url = "jdbc:postgresql://localhost:5432/hotel_db";
   private static final String username = "postgres";
   private static final String password = "your_password";

4. Compile and run the Java file:
   ```bash
   javac HotelReservationSystem.java
   java HotelReservationSystem

---

## 🙋‍♂️ Made By

**👨‍💻 Gaurav Vashistha**   
📧 [LinkedIn Profile]([https://www.linkedin.com/in/gaurav-vashistha/](https://www.linkedin.com/in/gaurav--vashistha/))
   
