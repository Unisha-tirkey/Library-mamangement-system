# Library Management System using C++

## Project Overview
The **Library Management System using C++** is a console-based application developed to automate and manage essential library operations.  
This project integrates **C++ programming** with a **MySQL database** to store and manage data related to books, members, and borrowing transactions.

---

## Technologies Used
- Programming Language: C++  
- Database: MySQL  
- Database Connector: MySQL Connector/C++  
- Application Type: Console-Based Application  

---

## Prerequisites
Before running this application, ensure that the following software is installed on your system:

- MySQL Server  
- MySQL Connector/C++  

Both can be downloaded and installed from the official MySQL website:  
https://dev.mysql.com/downloads/installer/

---

## Software Versions Used
- MySQL Server: 8.0.30  
- MySQL Connector/C++: 8.0.30  

---

## Database Configuration
Update the database connection credentials in the source code according to your local MySQL setup:

```cpp
const char* HOST = "localhost";       // Database host
const char* USER = "your_username";   // MySQL username
const char* PASSWD = "your_password"; // MySQL password
const char* DB_NAME = "your_db_name"; // Database name
const int PORT = 3306;                // Default MySQL port

```

Database Schema

The project includes a SQL file named library.sql, which contains all the queries required to create the database schema and tables used by the application.

Steps to set up the database:
1.Create a new database in MySQL
2.Execute the library.sql script
3.Verify that all required tables are created successfully

Features
Book Management
- Add new books to the library
- Display all books with title, author, and genre
- View the last 20 added or borrowed books
- Identify the most frequently borrowed books

Member Management
- Register new library members
- Display the most active members
- View all members along with the books they have borrowed (pending)

Borrowing and Returning System
- Borrow books from the library
- Return borrowed books
- Prevent borrowing of books that are already issued
- Restrict members to a maximum of five borrowed books

Project Objectives
- To design and implement a Library Management System using C++
- To perform database-driven operations using MySQL
- To apply real-world constraints and business logic in software development
- To enhance understanding of C++ and Database Management Systems

Future Enhancements
- Completion of pending member-book mapping feature
- Improved error handling and input validation
- Role-based user authentication
- Enhanced user interface
- Conversion to a graphical user interface (GUI) application
