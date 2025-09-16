# 🏦 Bank Class Implementation (Python OOP Exercise)

## 📌 Overview
This project demonstrates the use of **Object-Oriented Programming (OOP)** principles in Python, specifically **abstract base classes (ABC)**, **inheritance**, and **method overriding**.  

The exercise simulates a simple banking system with a **generic Bank class** and a **Swiss Bank implementation** that allows withdrawals.

---

## 💡 Key Learning

- How to define and use abstract base classes in Python.

- Enforcing method implementation in child classes.

- Practical use of inheritance and method overriding.

- Basic simulation of banking operations.

---

## 🔧 Tech Stack

- Language: Python 3

- Libraries: abc (Abstract Base Classes)

---

## 🛠️ Code Structure
### 1. `Bank` (Abstract Class)
- Defined as an abstract base class (inherits from `ABC`).
- Contains:
  - `basicinfo()` → Prints and returns generic bank info.  
  - `withdraw(amount)` → Abstract method to enforce implementation in child classes.

### 2. `Swiss` (Concrete Class)
- Inherits from `Bank`.  
- Has an initial balance of **1000 units**.  
- Methods:
  - `basicinfo()` → Prints and returns Swiss Bank details with current balance.  
  - `withdraw(amount)` → Handles withdrawal logic, validates sufficient balance.

### 3. `main()` (Driver Code)
- Ensures `Bank` is a subclass of `ABC`.  
- Creates a `Swiss` object and demonstrates:
  - Checking bank info  
  - Withdrawing funds  
  - Handling insufficient funds  

---

## 🚀 Example Run
```python
This is the Swiss Bank
Swiss Bank: 1000
Withdrawn amount: 100
New Balance: 900
Insufficient funds
