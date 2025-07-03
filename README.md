# 🔗 SQL Joins Practice (INNER, LEFT, RIGHT, FULL)

A beginner-friendly SQL practice project focused on mastering *JOINs* using real-world-style sample tables (Customers & Orders). This project helps in learning how to merge data from multiple tables using various SQL join types.

---

## 📌 Objective

- Learn how to *combine data* using INNER, LEFT, RIGHT, and FULL OUTER JOIN.
- Understand how different join types impact your result set.

---

## 🛠 Tools Used

- *DB Browser for SQLite*
- *MySQL Workbench*

---

## 📁 Tables Overview

- Customers – Contains customer details
- Orders – Contains product purchase details

---

## 🔍 Join Types Practiced

- INNER JOIN
- LEFT JOIN
- RIGHT JOIN (not supported in SQLite, tested in MySQL)
- FULL OUTER JOIN (emulated in SQLite using UNION)

---

## 🖼 Screenshots

### 📸 1. Inner join
![Inner Joins](https://github.com/9A-Ayush/task-5-joins-in-sql/blob/main/ss/Screenshot%202025-07-03%20143614.png)

### 📸 2. Left Outer JOIN Output
![Left outer join ](https://github.com/9A-Ayush/task-5-joins-in-sql/blob/main/ss/Screenshot%202025-07-03%20143900.png)

### 📸 3. Right Outer JOIN / UNION Output
![Right Outer join ](https://github.com/9A-Ayush/task-5-joins-in-sql/blob/main/ss/Screenshot%202025-07-03%20143917.png)

---

## 📦 Sample Queries

sql
-- INNER JOIN
SELECT Customers.CustomerName, Orders.Product
FROM Customers
INNER JOIN Orders ON Customers.CustomerID = Orders.CustomerID;

-- LEFT JOIN
SELECT Customers.CustomerName, Orders.Product
FROM Customers
LEFT JOIN Orders ON Customers.CustomerID = Orders.CustomerID;

-- FULL JOIN (SQLite workaround)
SELECT Customers.CustomerName, Orders.Product
FROM Customers
LEFT JOIN Orders ON Customers.CustomerID = Orders.CustomerID
UNION
SELECT Customers.CustomerName, Orders.Product
FROM Customers
RIGHT JOIN Orders ON Customers.CustomerID = Orders.CustomerID;


---

## 🎓 Outcome

✅ Mastery of how to merge and relate data across multiple tables using SQL joins.

---

## 📬 Contact

Feel free to reach out or drop a ⭐ if this helped!
