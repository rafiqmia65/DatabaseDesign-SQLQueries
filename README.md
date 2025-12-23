# 🚗 Vehicle Rental System – Database Design & SQL Queries

---

## 📌 Project Overview

The goal of this project is to design a simplified **Vehicle Rental System database** and write SQL queries to retrieve meaningful information from it.

Through this assignment, the following concepts are practiced:

- ERD design with proper relationships
- Primary Key and Foreign Key usage
- Writing SQL queries using `JOIN`, `EXISTS`, `WHERE`, `GROUP BY`, and `HAVING`
- Understanding real-world database business rules

---

## 🧩 System Modules

The system manages three core entities:

1. **Users** – Admins and Customers
2. **Vehicles** – Cars, Bikes, and Trucks
3. **Bookings** – Rental records connecting users and vehicles

---

## 🗂️ Database Design (ERD)

### Tables Included

- `users`
- `vehicles`
- `bookings`

### Relationships

- **One-to-Many**: One user can make multiple bookings
- **Many-to-One**: Many bookings can reference the same vehicle

### ERD Features

- Primary Keys (PK)
- Foreign Keys (FK)
- Relationship cardinality
- Status fields (booking status, vehicle availability)

🔗 **ERD Tool Used:** drawSQL ( https://drawsql.app/teams/rafiqs-team-1/diagrams/vehicle-rental-system )

---

## 📁 Repository Structure

```
DatabaseDesign-SQLQueries/
│
├── README.md          # Project documentation
├── queries.sql        # All SQL queries for Part 2

```

---

## 🧪 Part 2: SQL Queries Explanation

All required SQL queries are written in the `queries.sql` file. Below is a brief explanation of each query.

---

### 🔹 Query 1: INNER JOIN

**Purpose:** Retrieve booking information along with customer name and vehicle name.

**Concept Used:** `INNER JOIN`

This query joins the `bookings`, `users`, and `vehicles` tables to show complete booking details.

---

### 🔹 Query 2: NOT EXISTS

**Purpose:** Find all vehicles that have never been booked.

**Concept Used:** `NOT EXISTS`

This query checks for vehicles whose IDs do not appear in the `bookings` table.

---

### 🔹 Query 3: WHERE Clause

**Purpose:** Retrieve all available vehicles of a specific type (e.g., cars).

**Concept Used:** `SELECT`, `WHERE`

This query filters vehicles based on availability status and vehicle type.

---

### 🔹 Query 4: GROUP BY & HAVING

**Purpose:** Find vehicles that have been booked more than two times.

**Concept Used:** `GROUP BY`, `HAVING`, `COUNT`

This query groups bookings by vehicle and filters only those with more than two bookings.

---

## 🎤 Part 3: Theory Questions (Viva Practice)

The viva section focuses on understanding core database concepts. Answers are prepared in simple language and recorded as a video.

### Questions Covered

1. What is a foreign key and why is it important?
2. Difference between WHERE and HAVING clauses
3. What is a primary key and its characteristics
4. Difference between INNER JOIN and LEFT JOIN

🎥 **Viva Video Language:** Bengali

---

```
GitHub Repo: https://github.com/rafiqmia65/DatabaseDesign-SQLQueries.git
ERD Link: https://drawsql.app/teams/rafiqs-team-1/diagrams/vehicle-rental-system
Viva Video Link: https://drive.google.com/file/d/1TTCHmo6UxAlEGV8wn5YKPKNcP-hQCcsC/view
```
