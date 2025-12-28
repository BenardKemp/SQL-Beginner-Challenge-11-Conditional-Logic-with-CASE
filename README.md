# SQL Beginner Challenge #11: Conditional Logic with CASE

**Difficulty:** Beginner  
**Estimated time:** 15–20 minutes  
**Concepts:** `CASE`, conditional logic, derived columns  

This challenge introduces the `CASE` expression, which allows you to apply conditional logic directly inside SQL queries.

---

## 🧠 The Problem

A product manager asks:

> “Can we label products as **Cheap**, **Standard**, or **Expensive** based on their price?”

Instead of doing this logic in a spreadsheet or application code, you’ll handle it **inside SQL** using a `CASE` expression.

---

## 📊 Table Schema

### `products`

| Column Name | Type | Description |
|------------|------|-------------|
| product_id | INTEGER | Unique product ID |
| name | TEXT | Product name |
| category | TEXT | Product category |
| price | DECIMAL | Product price |

---

## 🧪 Sample Data

| product_id | name | category | price |
|-----------:|------|----------|------:|
| 101 | Wireless Mouse | Accessories | 24.99 |
| 102 | Mechanical Keyboard | Accessories | 89.00 |
| 103 | 27-inch Monitor | Displays | 229.99 |
| 104 | USB-C Hub | Accessories | 34.50 |
| 105 | Laptop Stand | Workspace | 39.99 |

---

## ✅ Requirements

Your query must:

- Return:
  - `name`
  - `price`
  - A derived column named `price_category`
- Use a `CASE` expression
- Apply the following rules:
  - Price < 50 → `Cheap`
  - Price between 50 and 150 → `Standard`
  - Price > 150 → `Expensive`
- Not use `SELECT *`

---

## ✍️ Your Task

Write a SQL query that fulfills the requirements.

```sql
-- Write your query here

