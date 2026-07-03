# Database-programming-group-assignment-

# Student Information Management System

## Project Overview
This database application is designed to manage and automate academic and financial records for an educational institution. Developed using SQL and PL/SQL, the application handles core student management operations, tracks course modules, automates tuition fee calculations based on registered credits, and processes student academic performance metrics.

## Core Features Implemented

* **Relational Schema**
The database consists of three interconnected tables (Students, Courses, and Enrollments) that enforce data integrity through primary keys, foreign keys, and structural constraints.

* **Database Function (CalculateTuition)**
A modular PL/SQL function that takes a student's ID as an input, dynamically matches their course enrollments with the credit structures, and returns the total calculated tuition fee.

* **Stored Procedure (UpdateStudentTuition)**
A reusable database procedure that automates administrative tasks by calling the calculation function and directly updating the student's financial records in the system.

* **Window Functions**
The application utilizes advanced SQL analytical window functions (DENSE_RANK and AVG OVER) to calculate real-time performance rankings and course averages without collapsing individual student records or disrupting the primary data views.

* **Anonymous PL/SQL Block**
A complete execution block that acts as the driver program. It implements a database cursor loop to automatically process financial updates for every student profile and prints an advanced performance and analytics report using console output.
