# Jail-Database-Management-System
Jail Database Management System
# 🏛️ JAIL DBMS – Jail Database Management System


A secure, role-based Jail Database Management System (JDMS) designed to digitize correctional facility operations, streamline administration, and improve transparency between prison administrators and inmates.

---

## 📌 Project Overview

The **Jail Database Management System (JDMS)** modernizes traditional manual record-keeping systems in correctional facilities by introducing:

- 🔐 Secure Role-Based Authentication  
- 📊 Admin Management Dashboard  
- 👤 Prisoner Portal  
- 🗂️ Structured Database with 3NF Normalization  
- 🛡️ SQL Injection Protection using Prepared Statements  
- ⚙️ Real-time Data Synchronization  

The system ensures **data integrity**, **security**, and **efficient administrative workflows**.

---

## 🎯 Objectives

- Replace manual jail record systems with a digital DBMS
- Ensure secure access for Admin and Prisoner roles
- Maintain prisoner records, sentences, behavior, parole decisions
- Implement ACID-compliant transactions
- Enforce database normalization (up to 3NF)

---

## 👥 Team Members & Contributions

| ID | Name | Contributions |
|----|------|--------------|
| 22341009 | Mujahidul Haque Jihad | Database creation, `db.php` connection, Prisoner dashboard, Prisoner profile, Edit prisoner |
| 23301039 | Ahmed Rakin | Login system, Logout function, Prisoner Parole module |
| 20201211 | Amreen Hassan | Admin Dashboard, Add Prisoner, Evaluate Prisoner |

---

## 🧩 System Architecture

The system follows a **Dual-Interface Architecture**:

### 🔹 Admin Interface
- Manage prisoner records
- Assign duties
- Evaluate behavior
- Make parole decisions
- Monitor system activity

### 🔹 Prisoner Portal
- View sentence details
- Request duty assignments
- View parole status
- Access personal profile

---

## 🗄️ Database Design

The database schema is normalized up to **Third Normal Form (3NF)**.

### 📂 Core Tables

- `Prisoner`
- `Security_Level`
- `Prisoner_Status`
- `Behaviour_Record`
- `Sentence`
- `Sentence_Type`
- `User_Account`
- `Role`
- `Admin`
- `Prisoner_User`
- `Parole_Evaluation`
- `Parole_Decision`
- `Duty_Assignment`
- `Crime`
- `Crime_Type`
- `Severity_Type`

### 🧱 Normalization

- ✅ **1NF:** No repeating groups; atomic attributes  
- ✅ **2NF:** No partial dependencies  
- ✅ **3NF:** No transitive dependencies  

The schema ensures minimal redundancy and strong relational integrity.

---

## 💻 Tech Stack

### Frontend
- HTML5
- CSS3
- PHP

### Backend
- PHP
- MySQL
- SQL (JOIN operations, constraints, transactions)

### Security Features
- Session-based authentication (`session_start`)
- Role-based access control
- Prepared statements (SQL injection prevention)

---

## 🔐 Authentication Flow

1. User logs in through `login.php`
2. Credentials validated against `User_Account` table
3. Session created
4. User redirected based on role:
   - Admin → `admin_dashboard.php`
   - Prisoner → `prisoner_dashboard.php`
5. Logout destroys session securely

---

## 📊 Features Breakdown

### 👮 Admin Features
- Add new prisoner
- Evaluate prisoner performance
- Assign duty
- Manage parole decisions
- View prisoner records

### 👤 Prisoner Features
- View sentence details
- Request duty assignments
- Track parole eligibility
- View profile & behavior points

---

## 🗃️ ER & Schema Design

- Designed using ER/EER modeling principles
- Implemented relational schema with foreign key constraints
- Enforced referential integrity across all major tables

---

## ⚙️ Installation Guide

### 🔹 Requirements
- XAMPP / WAMP
- PHP 7+
- MySQL
- Web Browser

### 🔹 Setup Steps

1. Clone the repository:

```bash
git clone https://github.com/mujahidulhaquejihad/JAIL-DBMS.git
