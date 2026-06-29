## Project Overview

This project demonstrates basic SQL operations using PostgreSQL. The database contains a Products table and implements CRUD (Create, Read, Update, Delete) operations for managing product records.

### Completed Tasks

* Create Product Database
* Create Products Table
* Insert Product Records
* Retrieve Product Records
* Update Product Records
* Delete Product Records
* SQL Documentation

---

## Technologies Used

* PostgreSQL 18
* pgAdmin 4
* SQL

---

## Database Structure

### Database Name

```sql
product_db
```

### Products Table

```sql
CREATE TABLE products (
    product_id SERIAL PRIMARY KEY,
    product_name VARCHAR(100) NOT NULL,
    category VARCHAR(100),
    price NUMERIC(10,2),
    stock INTEGER
);
```

### Table Columns

| Column Name  | Data Type     | Description      |
| ------------ | ------------- | ---------------- |
| product_id   | SERIAL        | Primary Key      |
| product_name | VARCHAR(100)  | Product Name     |
| category     | VARCHAR(100)  | Product Category |
| price        | NUMERIC(10,2) | Product Price    |
| stock        | INTEGER       | Available Stock  |

---

## CRUD Operations

### 1. Create (Insert)

```sql
INSERT INTO products
(product_name, category, price, stock)
VALUES
('Laptop', 'Electronics', 55000, 10);
```

### Output

| product_id | product_name | category    | price    | stock |
| ---------- | ------------ | ----------- | -------- | ----- |
| 1          | Laptop       | Electronics | 55000.00 | 10    |

---

### 2. Read (Select)

```sql
SELECT * FROM products;
```

### Result

Displays all available products in the table.

---

### 3. Update

```sql
UPDATE products
SET price = 60000
WHERE product_id = 1;
```

### Result

Product price updated successfully.

---

### 4. Delete

```sql
DELETE FROM products
WHERE product_id = 1;
```

### Result

Product record deleted successfully.

---

## How to Run

### Step 1

Open PostgreSQL or pgAdmin 4.

### Step 2

Create Database:

```sql
CREATE DATABASE product_db;
```

### Step 3

Connect to Database:

```sql
\c product_db
```

### Step 4

Create Products Table.

### Step 5

Execute Insert Query.

### Step 6

Execute Select Query to verify data.

### Step 7

Execute Update Query.

### Step 8

Execute Delete Query.

---

## Project Folder Structure

```text
BE-D9-002_Vinay/
│
├── product_database.sql
├── product_insert.sql
├── product_select.sql
├── product_update.sql
├── product_delete.sql
├── README.md
└── Screenshots/
```

---

## Screenshots Included

* Product Database Creation
* Product Table Creation
* Insert Query Output
* Select Query Output
* Update Query Output
* Delete Query Output

