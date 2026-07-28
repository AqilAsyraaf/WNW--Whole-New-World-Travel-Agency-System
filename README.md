# Whole New World (WNW) Travel Agency System

> **CSC264 - Introduction to Web and Mobile Application (Final Group Project)**  
> **Faculty of Computer and Mathematical Sciences, Universiti Teknologi MARA (UiTM) Campus Jasin**

---

## 📌 Project Overview

**Whole New World (WNW) Travel Agency System** is a responsive, full-stack web application designed to streamline travel booking and management operations for travel agencies and their clients. The system bridges traditional manual travel booking processes with a modern digital platform, allowing customers to easily browse travel packages, place reservations, track booking statuses, and submit support inquiries online.

For travel agency administrators and staff, the system provides a centralized dashboard to manage package listings, handle customer reservations, manage registered user accounts, and resolve incoming inquiries efficiently.

---

## 👥 Group Members & Information

* **Course:** CSC264 - Introduction to Web and Mobile Application
* **Program:** Diploma in Computer Science (CDCS110)
* **Class:** M3CDCS1104G
* **Lecturer:** Pn. Nurulhuda binti Ghazali
* **Submission Date:** 21 June 2026

### Team Members
| Name | Student ID |
| :--- | :--- |
| **Ahmad Baqir bin Azman** | 2024802256 |
| **Azim Hazmi bin Hasmariza** | 2024439304 |
| **Muhammad Aqil Asyraaf bin Hamri** | 2024246154 |
| **Mohd Zafran Zaim bin Mohd Ariff** | 2024695032 |

---

## ✨ Key Features

### 👨‍💼 Customer Features
- **Account Registration & Login:** Secure account creation and login with role-based navigation.
- **Interactive Package Browsing:** View available tour packages with pricing, duration, itineraries, and inclusions.
- **Dynamic Travel Booking:** Select travel packages, specify traveler numbers (adults, children, infants, elders), choose payment methods (Credit/Debit Card, Online Banking, Pay at Agency), and submit reservations.
- **Booking Management:** Track active bookings and history, with options to cancel active bookings.
- **Support & Inquiries:** Submit inquiries or support tickets and view response status (*Pending* / *Settled*).
- **User Profile:** Manage profile details and track personal activity history.

### 🛠️ Admin & Staff Features
- **Centralized Admin Dashboard:** Macro-level dashboard showing key system metrics (total users, active packages, bookings, inquiries).
- **Travel Package Management (CRUD):** Add, update, view, and delete travel packages including pricing tiers, descriptions, itineraries, and media.
- **Booking Management:** Review customer bookings, monitor travel dates, and update/cancel booking statuses.
- **Customer Management:** View registered customer accounts, contact numbers, and login timestamps.
- **Inquiry Management:** Read customer support messages, issue staff replies, and mark inquiries as *Settled*.

---

## 💻 Tech Stack

- **Frontend:** HTML5, CSS3 (Responsive Design), JavaScript (ES6+, DOM Manipulation, `localStorage`, Fetch API)
- **Backend:** PHP (Server-side handling, Session & Auth logic, MySQLi)
- **Database:** MySQL / MariaDB (`wnw_travel`)
- **Server Environment:** XAMPP / Apache

---

## 🗄️ Database Architecture (`wnw_travel`)

The database consists of 4 main relational tables:

1. **`user`**: Stores account credentials, contact info, and roles (`customer`, `admin`, `staff`).
2. **`packages`**: Holds package catalogue details, destinations, duration, images, itineraries, and pricing tiers (`self_tour_price`, `group_tour_price`, `private_tour_price`, `premium_private_tour_price`).
3. **`bookings`**: Stores customer reservation records linked via `username` and `package_key`, tracking traveler breakdown, travel date, payment method, and booking status (`Active`, `Cancelled`, `Completed`).
4. **`inquiries`**: Records customer support tickets, messages, admin replies, and status (`Pending`, `Settled`).

---

## 🚀 Installation & Local Setup

1. **Prerequisites:**
   - Install **XAMPP** (with Apache & MySQL enabled).

2. **Database Setup:**
   - Open **phpMyAdmin** (`http://localhost/phpmyadmin`).
   - Create a new database named `wnw_travel`.
   - Import the database structure and SQL tables provided in the project source.

3. **Deploy Web Project:**
   - Place the project folder into your XAMPP `htdocs` directory (e.g., `C:/xampp/htdocs/wnw_travel/`).

4. **Launch Application:**
   - Start Apache and MySQL modules in XAMPP Control Panel.
   - Open your web browser and navigate to `http://localhost/wnw_travel/index.html` or `http://localhost/wnw_travel/user.html`.

---

## 📄 License & Acknowledgements

Developed as part of the **CSC264 Final Semester Group Project** at **Universiti Teknologi MARA (UiTM) Campus Jasin**. Special thanks to **Pn. Nurulhuda binti Ghazali** for guidance and support throughout the course.
