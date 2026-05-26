# 📋 Registration Form Management System

![Python](https://img.shields.io/badge/Python-3.12-blue)
![MySQL](https://img.shields.io/badge/MySQL-8.0-orange)
![Tkinter](https://img.shields.io/badge/Tkinter-GUI-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

A **Python Tkinter Registration App** connected to a MySQL database. Users can register their personal details through a clean GUI form, and all information is stored securely in the `register` table of the `regi` MySQL database.

---

## 📸 Screenshots

### Main Registration Form
![Main Form](screenshots/main%20op.png)

### Filling In Details
![Inserting Data](screenshots/inserting%20the%20data%20.png)

### Successful Registration Message
![Success](screenshots/sucessfully.png)

### MySQL Query Output
![MySQL Query](screenshots/mysql%20query.png)

### Data Stored in Database
![Done](screenshots/done.png)

---

## ✨ Features

- Full user registration form with:
  - First Name and Surname
  - Email Address
  - Date of Birth (Day, Month, Year dropdowns)
  - Gender selection (Male, Female, Other)
  - Password with confirmation matching
- Confirmation checkbox before submitting
- Live MySQL database connection — data saved instantly on sign up
- Password mismatch validation with warning popup
- Form resets automatically after successful registration
- Success and error message popups for user feedback

---

## 🗄️ Database Schema

**Database:** `regi`  
**Table:** `register`

| Column | Type |
|---|---|
| user_names | VARCHAR(50) |
| user_surnames | VARCHAR(50) |
| user_emails | VARCHAR(50) |
| user_dd | VARCHAR(20) |
| user_mm | VARCHAR(20) |
| user_yy | VARCHAR(20) |
| user_passwords | VARCHAR(50) |
| user_genders | VARCHAR(50) |

### MySQL Setup Query

```sql
CREATE DATABASE regi;

USE regi;

CREATE TABLE register (
    user_names      VARCHAR(50),
    user_surnames   VARCHAR(50),
    user_emails     VARCHAR(50),
    user_dd         VARCHAR(20),
    user_mm         VARCHAR(20),
    user_yy         VARCHAR(20),
    user_passwords  VARCHAR(50),
    user_genders    VARCHAR(50)
);
```

---

## ⚙️ Requirements

- Python 3.x (tested with 3.12)
- Tkinter (comes built-in with Python)
- MySQL Server 8.0
- mysql-connector-python

---

## 📦 Installation

**1. Clone the repository**
```bash
git clone https://github.com/sakshi-mohite01/your-repo-name.git
cd your-repo-name
```

**2. Install the required Python library**
```bash
pip install mysql-connector-python
```

**3. Set up MySQL database**

Open MySQL and run the setup queries from the Database Schema section above.

**4. Update your database credentials**

Open the Python file and update this line with your MySQL username and password:
```python
con = m.connect(host='localhost', user='root', passwd='your_password', database='regi')
```

**5. Run the application**
```bash
python registration.py
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Tkinter | GUI framework for the registration form |
| MySQL | Relational database for storing user data |
| mysql-connector-python | Python-MySQL database connectivity |

---

## 📚 What I Learned

- Connecting Python applications to a MySQL relational database
- Designing and querying database schemas using SQL
- Building GUI applications using Tkinter widgets and layout managers
- Implementing form validation logic (password matching, checkbox confirmation)
- Handling live database INSERT operations and connection management

---

## 👩‍💻 Author

**Sakshi Devendra Mohite**  
MSc Data Science — University of Greenwich  
[LinkedIn](https://www.linkedin.com/in/sakshi-mohite03) | [GitHub](https://github.com/sakshi-mohite01)
