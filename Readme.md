# Inventory Management System

## 📌 Project Overview

This is a simple **Inventory Management System** implemented in Python. The system allows users to add, remove, and track inventory items. The project has been improved by applying static analysis best practices using tools such as **Pylint**, **Bandit**, and **Flake8**.

The updated version follows Python best practices, improves code readability, and eliminates major security concerns (such as the use of `eval()`).

---

## ✅ Features

* Add new items with quantity
* Remove items safely
* Load and save inventory to a JSON file
* Display current inventory
* Identify low-stock items
* Logging added for improved debugging
* Static analysis compliance

---

## 🧩 Module & Function Documentation

| Function Name     | Description                              | Parameters                            | Returns |
| ----------------- | ---------------------------------------- | ------------------------------------- | ------- |
| `add_item`        | Adds a specified quantity of an item     | `item: str`, `qty: int`, `logs: list` | None    |
| `remove_item`     | Removes quantity of an item, logs errors | `item: str`, `qty: int`               | None    |
| `get_qty`         | Retrieves quantity of an item            | `item: str`                           | int     |
| `load_data`       | Loads inventory data from JSON           | `file: str`                           | None    |
| `save_data`       | Saves inventory data to JSON             | `file: str`                           | None    |
| `print_data`      | Displays current inventory               | None                                  | None    |
| `check_low_items` | Returns items below a quantity threshold | `threshold: int`                      | list    |
| `main`            | Entry point for executing program logic  | None                                  | None    |

---

## 📂 Project Structure

```
📁 inventory_system
├── inventory_system.py
├── inventory.json (auto-created)
└── README.md
```

---

## 🛠 Static Analysis Summary

| Tool       | Purpose                | Result Summary              |
| ---------- | ---------------------- | --------------------------- |
| **Pylint** | Code quality & style   | Score improved after fixes  |
| **Flake8** | PEP8 compliance        | Long lines and blanks fixed |
| **Bandit** | Security vulnerability | Removed `eval`, no issues   |

---

## 🚀 How to Run the Project

### **1. Run Locally**

```bash
python inventory_system.py
```

### **2. Run Static Analysis**

```bash
pylint inventory_system.py
flake8 inventory_system.py
bandit -r inventory_system.py
```

---

## 🧠 Personal Reflection

### 🔷 What I Improved

* Fixed naming conventions to follow snake_case.
* Removed insecure `eval()` usage.
* Added logging for better debugging.
* Used `with open()` to prevent resource leakage.

### 🔷 Challenges Faced

* Initial errors with missing module and syntax formatting.
* Understanding Pylint and Bandit reports took time.

### 🔷 Future Enhancements

* Convert script into a class-based system
* Add exception handling in `main()`
* Build a simple CLI or web interface

---


# Inventory Management System

---

## 🔷 1. Module Documentation Table

| Module/File Name      | Description                                                          | Key Functions/Classes                                                                                         | Input                             | Output                          | Dependencies              |
| --------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | --------------------------------- | ------------------------------- | ------------------------- |
| `inventory_system.py` | Core module that manages inventory items, quantities, and operations | `Inventory` class, `add_item()`, `remove_item()`, `update_quantity()`, `search_item()`, `display_inventory()` | User input or function parameters | Console output or return values | Python 3.x, `json` module |

---

## 🔷 2. Pylint, Bandit & Flake8 Summary Table

| Tool       | Purpose                                | Command Used                    | Result Summary              | Interpretation                            |
| ---------- | -------------------------------------- | ------------------------------- | --------------------------- | ----------------------------------------- |
| **Pylint** | Checks code quality, style, and errors | `pylint inventory_system.py`    | Passed with improved score  | Code is clean and follows standards       |
| **Bandit** | Scans for security vulnerabilities     | `bandit -r inventory_system.py` | No security issues detected | Secure code with no harmful usage         |
| **Flake8** | Ensures PEP 8 compliance               | `flake8 inventory_system.py`    | No warnings/errors reported | Code adheres to industry style guidelines |

✅ **Overall Status:** Passed quality, security, and style checks successfully.

---

## 🔷 3. Personal Reflection (Detailed & Professional)

### **Q1. Purpose of this Project**

The goal of this project was to design a simple inventory management system to track items, manage stock quantities, and provide real-time updates, simulating real-world warehouse or retail operations.

### **Q2. Challenges Faced and Solutions**

The major challenge was maintaining code readability and structure. Initially, I faced multiple linting issues. Through the use of static analysis tools like Pylint and Flake8, I resolved these and improved maintainability.

### **Q3. Ensuring Quality and Security**

* **Pylint:** Enforced proper structure and naming conventions.
* **Flake8:** Ensured formatting according to PEP 8 standards.
* **Bandit:** Verified security, ensuring no unsafe or vulnerable coding practices.

### **Q4. What I Learned**

* Improved understanding of Python project structure.
* Importance of static analysis tools.
* Gained experience in exception handling and secure coding.

### **Q5. Future Improvements**

* Add persistent storage (JSON/SQLite)
* Implement GUI or web interface
* Create unit tests
* Add user authentication and access roles

---
## 📌 Expanded Project Documentation

### 🔷 Module Documentation Table

| Module/File Name      | Description                                                                                   | Key Functions/Classes                                                            | Input                    | Output                          | Dependencies            |
| --------------------- | --------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | ------------------------ | ------------------------------- | ----------------------- |
| `inventory_system.py` | Core module that manages inventory items, quantities, and operations like add, remove, search | add_item(), remove_item(), update_quantity(), search_item(), display_inventory() | User input or parameters | Console output or return values | Python 3.x, json module |

### 🔷 Static Analysis Tools Summary

| Tool   | Purpose                      | Command Used                  | Result Summary              | Interpretation              |
| ------ | ---------------------------- | ----------------------------- | --------------------------- | --------------------------- |
| Pylint | Code quality & style         | pylint inventory_system.py    | No major issues after fixes | Code follows best practices |
| Bandit | Security scanning            | bandit -r inventory_system.py | No vulnerabilities detected | Code is secure              |
| Flake8 | Formatting & PEP8 compliance | flake8 inventory_system.py    | No warnings                 | Code is well-formatted      |

✅ **Overall Status:** Passed code quality, security, and style checks successfully.

### 🔷 Detailed Personal Reflection

**Purpose:** Build a functional inventory system demonstrating real-world application and Python proficiency.
**Challenges Overcome:** Fixed linting errors, improved function structure, and removed security risks.
**Security & Quality Assurance:** Static tools enforced high standards and eliminated errors.
**Key Learnings:** Enhanced understanding of Python best practices and static analysis.
**Future Improvements:** Add database storage, GUI, unit tests, and role-based access control.

