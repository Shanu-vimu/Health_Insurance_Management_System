Health Insurance Management System | Official Repository 🌟
Welcome to the development repository for the Health Insurance Management System — a simple, human-centered PHP/MySQL portal that makes insurance tasks less painful and more transparent. This project is designed to help policyholders register, choose packages, submit claims, make payments, and raise complaints — while providing administrators an approachable dashboard for managing users, claims, and communications. 💼❤️

Why this project? 💡
Insurance processes can be frustrating. This system is a compact, easy-to-extend prototype that demonstrates the core flows of a small insurer: onboarding, claim lifecycle, payment tracking, and complaint handling. It's ideal for learning, prototyping, or as a base for a more robust production system.

Key features ✨

🔐 User registration & authentication (registration.php, login.php)
🧾 Claims management: submit, view, and track claims (claim_form.php, My Claims.php, admin_view_claims.php)
💳 Payment recording and history (payment.php, payment_db.php)
📣 Complaint & contact handling with admin review (complaint.php, contactus.php, admin_view_contact.php)
🛠️ Admin tools for user and complaint management (admindashboard.php, admin_edit_user.php, delete_complaint.php)
🗃️ Database schema and sample SQL in registration_db.sql
🧩 Reusable layout components in header.php and footer.php
Project structure (high level)
├── php — shared partials (header.php, footer.php)
├── css — styles for pages (homepage.css, claim.css, etc.)
├── js — small client scripts (passwordshow.js, contactus.js)
├── Database — SQL schema and table exports (registration_db.sql, per-table SQLs)
├── img, logo — media assets
├── root-level PHP pages — user/admin flows (registration.php, login.php, claim_form.php, admindashboard.php, ...)
├── con_db.php — central MySQL connection file (update DB credentials here)

Technology stack 🧭

Backend: Plain PHP (server-side rendering)
Database: MySQL (SQL files in Database)
Frontend: HTML/CSS (in css), small JavaScript utilities (in js)
Designed for deployment on local dev stacks like XAMPP / WAMP / Laragon (Windows)
Available pages (sample)

Public: Home Page.php, registration.php, login.php, Packages.php, claim_form.php, payment.php, contactus.php, complaint.php
User area: My Claims.php, view_complaints.php
Admin area: admindashboard.php, admin_view_claims.php, admin_view_contact.php, admin_edit_user.php, delete_complaint.php
Getting started (Windows / XAMPP) 🪟
Prerequisites

XAMPP, WAMP, or Laragon (PHP + MySQL)
Web browser (Chrome, Edge, Firefox)
Quick install and run

Start Apache and MySQL (use XAMPP Control Panel or equivalent).
Import the database:
Using phpMyAdmin: open http://localhost/phpmyadmin → create a database (e.g., insurance_db) → Import → choose registration_db.sql and run.
Or using the MySQL client in PowerShell:
Update database credentials in con_db.php to match your local MySQL user, password, and database name.
Place the project folder in your webserver doc root (e.g., C:\xampp\htdocs\Health_Insurance_Management_System-main) and open http://localhost/Health_Insurance_Management_System-main/ in your browser.
Use the admin pages (if an admin account exists in the DB) to review claims, contacts, and complaints.
