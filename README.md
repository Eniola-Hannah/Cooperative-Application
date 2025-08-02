# 🏦 Olive Lane Co-operative Network (Python CLI App)

Welcome to the **Olive Lane Co-operative Network** — a command-line interface (CLI) co-operative management system I built back in 2022. This project was my attempt to simulate a basic co-operative society model where users can save money, request loans, and manage membership details.

![co-operative-sociteies-solutions ](https://github.com/user-attachments/assets/3249caf1-3ef2-418c-b887-addebc014046)

---

## Features

- 👤 **New & Returning Member Workflow**
- 💰 **Savings Management** (Minimum ₦500 per meeting)
- 💳 **Loan Application & Repayment**
- 📊 **Balance Inquiry**
- 🧾 **Interest Calculation** (5% flat)
- 🧑🏾‍🤝‍🧑🏾 **Member Directory**
- 📢 **Weekly Notifications**

---

## Tech Stack

- **Python** (Core scripting)
- **MySQL** (Database operations)
- `mysql.connector` for database integration
- `numpy` for generating unique IDs
- `re` for input validation
- `time` & `sys` for CLI interaction & control

---

## How to Run

> **Note:** Ensure MySQL is set up and the database `OliveLane_cooperative_database` with the `lagos_branch` table exists.

```bash
1. Clone the repository:
   git clone https://github.com/your-username/olive-lane-cooperative.git

2. Open the script:
   cd olive-lane-cooperative
   python Co_operativeMachine.py
```

## Database Schema (Table: chicago_branch)
```sql
CREATE TABLE lagos_branch (
  customer_id INT AUTO_INCREMENT PRIMARY KEY,
  Full_Name VARCHAR(40),
  Contact VARCHAR(11),
  Username VARCHAR(20) UNIQUE,
  Address VARCHAR(50),
  Occupation VARCHAR(20),
  Savings INT,
  unique_ID VARCHAR(4) UNIQUE,
  Loan INT,
  Interest INT,
  loanBreakdown FLOAT,
  DueInterest FLOAT,
  Info VARCHAR(50)
);
```

## 📌 Notes
- This project was built in 2022 as a final project for completing python course. It is an insightful CLI app for managing a basic co-operative system.
- It’s not production-grade but serves as a great educational foundation for database operations and logic structuring in Python.

## Let's Connect
- 🌟[LinkedIn](linkedin.com/in/eniola-hannah)
