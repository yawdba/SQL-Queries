# E-Commerce Database SQL Queries

This repository contains SQL queries for analyzing and managing an e-commerce database. The dataset includes tables for products, clients, sales, suppliers, and employees. The queries cover a variety of tasks, from basic data retrieval to advanced analysis and reporting.

---

## Introduction

This project demonstrates SQL skills by solving real-world scenarios using an e-commerce database. The focus is on retrieving insights, performing calculations, and analyzing data relationships. The database schema includes the following tables:
- **Products**: Product details like name, category, price, and stock.
- **mkt_Clients**: Customer information.
- **mkt_Sales**: Sales records linking products and clients.
- **mkt_Suppliers**: Supplier information for products.
- **mkt_Employees**: Employee details.

---

## Database Schema

### Products
- `ProductID` (Primary Key)
- `ProductName`
- `Category`
- `Price`
- `StockQuantity`

### mkt_Clients
- `ClientID` (Primary Key)
- `FirstName`
- `LastName`
- `Email`
- `Phone`

### mkt_Sales
- `SaleID` (Primary Key)
- `SProductID` (Foreign Key)
- `ClientID` (Foreign Key)
- `SaleDate`
- `Quantity`
- `TotalAmount`

### mkt_Suppliers
- `SupplierID` (Primary Key)
- `SupplierName`
- `ContactPerson`
- `Email`
- `Phone`

### mkt_EmployeeDetails
- `EmployeeID` (Primary Key)
- `FirstName`
- `LastName`
- `Email`
- `Phone`

---

## Queries

### Basic Queries

1. Retrieve all product details sorted by category and price in descending order.
2. List all clients' first names, last names, and emails alphabetically by their last name.
3. Find all products with a stock quantity less than 20.

### Aggregation and Filtering

4. Calculate the total revenue generated from all sales.
5. Find the average price of products in the "Furniture" category.
6. Count how many products belong to each category.

### Joining Tables

7. Fetch all sales records with the corresponding product names and client names.
8. Identify which clients have purchased "Electronics" products.
9. List all sales where the total amount exceeds $500, including client and product details.

### Advanced Queries

10. Determine the top 3 best-selling products based on total quantity sold.
11. Retrieve clients who have not made any purchases.
12. Find products with low stock (less than 30 units) and their suppliers.

### Date-Based Analysis

13. List all sales that occurred in January 2024.

---

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ecommerce-database-sql.git

