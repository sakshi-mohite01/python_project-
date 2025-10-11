
# Tkinter Registration App

![Python](https://img.shields.io/badge/Python-3.12-blue)
![MySQL](https://img.shields.io/badge/MySQL-8.0-orange)
![Tkinter](https://img.shields.io/badge/Tkinter-GUI-green)

A **Python Tkinter Registration App** connected to a MySQL database.  
Users can register with their details, and the information is stored in the `register` table of the `regi` database.

---

## Features

- User registration with:
  - First Name, Surname, Email  
  - Date of Birth (Day, Month, Year)  
  - Gender  
  - Password with confirmation  
- Data is stored securely in MySQL  
- Simple and intuitive GUI with Tkinter

---

## Requirements

- Python 3.x (tested with 3.12)  
- Tkinter (comes with Python)  
- MySQL Server (8.0 recommended)  
- mysql-connector-python  

Install MySQL connector:

```bash
pip install mysql-connector-python



## Database Schema

**Table:** `register`

| Column      | Type          |
|------------|---------------|
| first_name | VARCHAR(50)   |
| surname    | VARCHAR(50)   |
| email      | VARCHAR(100)  |
| day        | INT           |
| month      | VARCHAR(20)   |
| year       | INT           |
| password   | VARCHAR(100)  |
| gender     | VARCHAR(10)   |

