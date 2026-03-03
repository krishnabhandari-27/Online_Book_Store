# 📚 Online Bookstore Database Management System (SQL Project)

## 📌 Project Overview

This project is a ** Online Bookstore Database Management System** built using SQL.  
It demonstrates database design, table relationships, and advanced querying using joins, aggregations, filtering, grouping, and sorting.

The system manages:

- 📖 Books
- 👤 Customers
- 🛒 Orders

This project showcases practical SQL skills required for Data Analyst and BI roles.

---

## 🗂️ Database Schema

The project contains 3 tables:

### 1️⃣ Books
| Column | Data Type | Description |
|--------|-----------|------------|
| Book_ID | SERIAL (PK) | Unique Book ID |
| Title | VARCHAR(100) | Book Title |
| Author | VARCHAR(100) | Author Name |
| Genre | VARCHAR(50) | Book Genre |
| Published_Year | INT | Year of Publication |
| Price | NUMERIC(10,2) | Book Price |
| Stock | INT | Available Stock |

---

### 2️⃣ Customers
| Column | Data Type | Description |
|--------|-----------|------------|
| Customer_ID | SERIAL (PK) | Unique Customer ID |
| Name | VARCHAR(100) | Customer Name |
| Email | VARCHAR(100) | Email Address |
| Phone | VARCHAR(15) | Contact Number |
| City | VARCHAR(50) | Customer City |
| Country | VARCHAR(150) | Customer Country |

---

### 3️⃣ Orders
| Column | Data Type | Description |
|--------|-----------|------------|
| Order_ID | SERIAL (PK) | Unique Order ID |
| Customer_ID | INT (FK) | References Customers |
| Book_ID | INT (FK) | References Books |
| Order_Date | DATE | Date of Order |
| Quantity | INT | Number of Books Ordered |
| Total_Amount | NUMERIC(10,2) | Total Price |

---

## 🔗 Relationships

- `Orders.Customer_ID` → references `Customers.Customer_ID`
- `Orders.Book_ID` → references `Books.Book_ID`

This ensures proper relational database integrity.

---

## 🧠 SQL Concepts Used

This project includes:

- ✅ CREATE TABLE
- ✅ PRIMARY KEY & FOREIGN KEY
- ✅ SELECT queries
- ✅ WHERE conditions
- ✅ BETWEEN operator
- ✅ GROUP BY
- ✅ HAVING clause
- ✅ ORDER BY
- ✅ LIMIT
- ✅ DISTINCT
- ✅ Aggregate Functions (SUM, AVG, COUNT)
- ✅ JOIN operations

---

## 📊 Business Queries Implemented

Some key analytical queries included in this project:

1. Retrieve books by genre  
2. Find books published after a specific year  
3. Get customers from a specific country  
4. Orders placed in a specific month  
5. Total stock available  
6. Most expensive book  
7. Customers with multiple orders  
8. Orders above a certain amount  
9. List all available genres  
10. Book with lowest stock  
11. Total revenue generated  
12. Total books sold by genre  
13. Average price by genre  
14. Customers with at least 2 orders  
15. Most frequently ordered book  
16. Top 3 most expensive fantasy books  
17. Total books sold per author  
18. Cities where high-spending customers are located  
19. Customer who spent the most  

---

## 💡 Skills Demonstrated

- Relational Database Design
- Data Aggregation & Analysis
- Business-Oriented Query Writing
- Data Filtering & Sorting
- Analytical Thinking using SQL

---

## 🛠️ Tools Used

- PostgreSQL / MySQL
