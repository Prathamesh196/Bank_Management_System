# 🏦 Java ATM Simulator – Desktop Banking Application

A **Java Swing desktop application** that simulates real ATM banking operations such as **User Registration, Login, Deposit, Withdrawal, Balance Inquiry, Mini Statement, and PIN Change** using **MySQL** as the backend database.

This project demonstrates how core banking workflows can be implemented using **Java (UI + Logic)** and **JDBC (Database Connectivity)** in a modular and practical way.

---

## 🚀 Features

| Module            | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| Sign-Up           | New user registration with personal details and secure 6-digit PIN         |
| Login             | Authentication using Card Number and PIN                                   |
| Deposit           | Add money to account and update balance                                    |
| Withdrawal        | Withdraw money and update balance                                          |
| Balance Inquiry   | Display current account balance                                            |
| Mini Statement    | Show recent transactions with date and amount                              |
| PIN Change        | Allow users to securely change PIN                                         |
| Validation        | Error prompts for invalid inputs, wrong PIN, or empty fields               |

---

## 🧰 Tech Stack

| Technology     | Purpose                                |
|----------------|-----------------------------------------|
| Java Swing     | GUI (User Interface)                   |
| MySQL          | Database storage                       |
| JDBC           | Java–MySQL connectivity                |
| JCalendar      | Date picker for Date of Birth input    |
| NetBeans IDE   | Development environment                |

---

## 🗃️ Database Schema

### `signup`

| Column          | Type        |
|-----------------|------------|
| formno          | VARCHAR(20)|
| name            | VARCHAR(20)|
| father_name     | VARCHAR(20)|
| dob             | VARCHAR(20)|
| gender          | VARCHAR(20)|
| email           | VARCHAR(30)|
| marital_status  | VARCHAR(20)|
| address         | VARCHAR(40)|
| city            | VARCHAR(25)|
| pincode         | VARCHAR(20)|
| state           | VARCHAR(25)|

### `signuptwo`

| Column          | Type        |
|-----------------|------------|
| formno          | VARCHAR(20)|
| religion        | VARCHAR(20)|
| category        | VARCHAR(20)|
| income          | VARCHAR(20)|
| education       | VARCHAR(20)|
| occupation      | VARCHAR(20)|
| pan             | VARCHAR(20)|
| aadhar          | VARCHAR(20)|
| seniorcitizen   | VARCHAR(20)|
| existingaccount | VARCHAR(20)|

### `signupthree`

| Column      | Type         |
|-------------|--------------|
| formno      | VARCHAR(20)  |
| accountType | VARCHAR(40)  |
| cardnumber  | VARCHAR(25)  |
| pin         | VARCHAR(10)  |
| facility    | VARCHAR(100) |

### `login`

| Column     | Type        |
|------------|------------|
| formno     | VARCHAR(20)|
| cardnumber | VARCHAR(25)|
| pin        | VARCHAR(10)|

### `bank`

| Column | Type        |
|--------|------------|
| pin    | VARCHAR(10)|
| date   | VARCHAR(50)|
| type   | VARCHAR(20)|
| amount | VARCHAR(20)|




🔄 Application Workflow
Step	Description
Sign-Up	User enters details and generates Card Number & PIN
Login	User logs in with Card Number and PIN
Deposit	Enter amount → balance increases
Withdrawal	Enter amount → balance decreases
Balance Inquiry	Displays current balance
Mini Statement	Displays recent transactions
PIN Change	User updates PIN securely

🎯 Learning Outcomes
Java Swing UI development

JDBC integration with MySQL

Handling transactions and validations

Building modular desktop applications

Implementing authentication systems

🔮 Future Enhancements
PIN encryption

Admin dashboard

Transaction export

Improved UI with JavaFX

Multi-user session handling

✅ Conclusion
This project provides a complete, working example of how ATM-style banking operations can be implemented in a desktop environment using Java and MySQL. It combines user interface design, database management, and transaction logic into a cohesive application and serves as a strong foundation for more advanced banking or financial software projects.
