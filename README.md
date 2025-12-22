# Vehicle Rental System

## Project Overview
This project is a simple Vehicle Rental System designed to demonstrate
basic database design and SQL querying concepts.

The system manages three core entities:
- Users
- Vehicles
- Bookings

It supports vehicle booking, availability tracking, and booking history
using relational database concepts.

---

## Database Design
The database contains three tables:

### Users
Stores user information such as name, email, phone number, and role
(Admin or Customer). Each user is uniquely identified by `user_id`.

### Vehicles
Stores vehicle details including name, type, model year, registration
number, rental price per day, and current availability status.

### Bookings
Stores booking information including which user booked which vehicle,
rental start and end dates, booking status, and total cost.

---

## Explanation of SQL Queries

### Query 1: INNER JOIN
This query retrieves booking details along with the customer name and
vehicle name by joining the `users`, `vehicles`, and `bookings` tables.

### Query 2: NOT EXISTS
This query finds all vehicles that have never been booked by checking
which vehicles do not exist in the `bookings` table.

### Query 3: WHERE Clause
This query retrieves all available vehicles of a specific type
(for example, cars).

### Query 4: GROUP BY and HAVING
This query counts total bookings for each vehicle and displays only
those vehicles that have more than two bookings.

---

## Conclusion
This project demonstrates the use of relational database design,
primary and foreign keys, and common SQL queries such as JOIN,
WHERE, EXISTS, GROUP BY, and HAVING.
