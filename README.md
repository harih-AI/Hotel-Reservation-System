# 🏨 Hotel Reservation System (Console-based with SQLite)

A simple, modular, and scalable Python console application for hotel room booking. Built using Object-Oriented Programming and follows SOLID design principles. Perfect for learning, interviews, and academic projects.

---

## 📌 Features

- 👤 Customer Registration and Login
- 🛏 View Available Rooms
- 📅 Book Rooms with Check-in/Check-out Dates
- ✅ SQLite Database Integration
- 🧱 Clean File Structure and Modular Code
- 💡 Designed with OOP, Encapsulation, Abstraction, Inheritance, and Polymorphism

## 🛠️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/hotel-reservation-system.git
cd hotel-reservation-system
````

### 2. Initialize the Database

```bash
sqlite3 hotel.db < schema.sql
```

### 3. Run the Application

```bash
python main.py
```

---

## 🧠 Example SQL Queries

```sql
-- 1. JOIN: See who booked what
SELECT u.name, r.room_type, b.check_in
FROM bookings b
JOIN users u ON b.user_id = u.user_id
JOIN rooms r ON b.room_id = r.room_id;

-- 2. GROUP BY: Room type counts
SELECT room_type, COUNT(*) FROM rooms GROUP BY room_type;

-- 3. Filter: Budget rooms
SELECT * FROM rooms WHERE price_per_night < 1500;
```

---

## 🔍 Concepts Used

* ✅ OOP: Class-based architecture
* ✅ SOLID Principles
* ✅ Encapsulation, Abstraction, Inheritance
* ✅ SQL Queries & Relational Design (ER Diagram)
* ✅ Console-based user interface
* ✅ Input validation & basic edge case handling

---

## 📈 Improvements (Next Steps)

* Admin Panel: Add/Edit/Delete Rooms
* View & Cancel Bookings
* Session-based login system
* Unit testing with `unittest`
* GUI/Web version using Flask or Tkinter

---

## 🧪 Testing Strategy

* Register/login success and failure
* Room booking success and availability change
* Edge case: Invalid input, reused emails

---

## 📄 License

This project is open-source and free to use under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

Designed for learning purposes, technical interviews, and academic project demos. Inspired by real-world software architecture principles.

---

