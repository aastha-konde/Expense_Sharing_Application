# SplitSmart – Expense Sharing Application using Java
---
> A Java-based desktop application for tracking and managing shared expenses, optimizing settlements, and enhancing financial transparency among groups.

## Introduction

Managing finances in group settings—such as trips, shared households, or friends dining out—can often become disorganized, error-prone, and time-consuming. Manual methods lead to confusion, disputes, and delays in settlements.

**SplitSmart** addresses this problem by offering a robust desktop solution built in Java. The application simplifies financial collaboration by allowing users to log personal and group expenses, track income, manage transfers, and automatically settle shared costs.

## Objective

* Track personal incomes, expenses, and transfers.
* Efficiently manage group expenses.
* Automate fair and minimized settlements.
* Ensure clarity and transparency in shared finances.
* Provide a secure, interactive, and intuitive desktop experience.

---

## Technology Stack

| Layer               | Technology Used         |
| ------------------- | ----------------------- |
| **Frontend (UI)**   | JavaFX + FXML + CSS     |
| **Business Logic**  | Java (OOP, Collections) |
| **Database Access** | JDBC                    |
| **Database**        | PostgreSQL              |
| **Build Tool**      | Maven                   |

---

## Features

### User Management

* Register, login, logout
* Password hashing for security
* Role-based access (admin/member)

### Group Management

* Create, edit, delete groups
* Dynamic member invitation/removal
* Assign roles: Creator, Editor, Viewer

### Expense Management

* Record personal & shared expenses
* Categorize by type/date/amount
* Support for equal, unequal, or percentage splits

### Settlement System

* Real-time balance tracking
* Graph-based optimization for minimal transactions
* Immediate or periodic debt clearance

---

## System Architecture

### Three-Tier Modular Design:

1. **Presentation Layer**

   * Built with JavaFX (FXML + CSS)
   * UI screens: Login, Dashboard, Expense Form, Group Manager
2. **Business Logic Layer**

   * Core services: authentication, calculations, role management
   * Implements splitting & settlement algorithms
3. **Data Access Layer (DAO)**

   * CRUD operations using JDBC
   * Prepared statements to prevent SQL injection

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/aastha-konde/Expense_Sharing_Application
cd Expense_Sharing_Application
```

### 2. Configure the Database

Edit the `DatabaseConfig.java` file:

```java
private static final String DB_URL = "YOUR_DB_URL";
private static final String DB_USER = "YOUR_USERNAME";
private static final String DB_PASSWORD = "YOUR_PASSWORD";
```

Make sure your PostgreSQL server is running and the schema is initialized.

### 3. Run the Application

Using Maven:

```bash
mvn clean javafx:run
```

---
