# 🚗 Vehicle Rental System - Database Design & SQL Queries

## 📌 Project Overview
This project is a simplified **Vehicle Rental System** designed to demonstrate core database concepts including **ERD design**, **primary and foreign key relationships**, and **SQL queries** using JOIN, EXISTS, WHERE, GROUP BY, and HAVING clauses.

The system manages users, vehicles, and bookings while maintaining proper relational integrity.

---

## 🎯 Objectives
- Design a relational database using ERD
- Understand 1-to-Many and Many-to-1 relationships
- Implement primary keys and foreign keys
- Write optimized SQL queries
- Practice viva concepts related to databases

---

## 🗂️ Database Entities

### 1️⃣ Users
Stores information about system users.
- id (UUID, Primary Key)
- role (Admin / Customer)
- name
- email (Unique)
- phone_number
- password

---

### 2️⃣ Vehicles
Stores vehicle-related information.
- id (UUID, Primary Key)
- name
- type (Car / Bike / Truck)
- model
- registration_number (Unique)
- price_per_day
- availability_status (Available / Rented / Maintenance)

---

### 3️⃣ Bookings
Stores booking details.
- id (UUID, Primary Key)
- user_id (Foreign Key → Users)
- vehicle_id (Foreign Key → Vehicles)
- start_date
- end_date
- status (Pending / Confirmed / Completed / Cancelled)
- total_cost

---

## 🔗 Database Relationships
- **One-to-Many**: One User can have multiple Bookings
- **Many-to-One**: Multiple Bookings can belong to one Vehicle
- **Logical One-to-One**: Each Booking is linked to one User and one Vehicle

---

## 🧠 SQL Queries Covered
- INNER JOIN
- NOT EXISTS
- WHERE filtering
- GROUP BY with HAVING

## Conclusion
This project demonstrates the use of relational database design, primary and foreign keys, and common SQL queries such as JOIN, WHERE, EXISTS, GROUP BY, and HAVING.
