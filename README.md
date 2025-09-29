# E-commerce Database Management System

## Author
Henok Girma

## Description
This repository contains a fully designed relational database schema for an E-commerce Store. The database includes tables for users, products, orders, categories, and the relationships between them.

## Tables
1. **Users**
   - Stores user information.
   - `userID` is the primary key.
2. **Products**
   - Stores product information including name, description, price, and stock.
   - `productID` is the primary key.
3. **Orders**
   - Stores orders made by users.
   - `orderID` is the primary key.
   - Linked to Users table via `userID`.
4. **OrderItems**
   - Handles the Many-to-Many relationship between Orders and Products.
   - Composite primary key: `orderID` + `productID`.
5. **Categories**
   - Stores product categories.
   - `categoryID` is the primary key.
6. **ProductCategories**
   - Handles the Many-to-Many relationship between Products and Categories.
   - Composite primary key: `productID` + `categoryID`.

## How to Run
1. Clone this repository:
   ```bash
   git clone <your-github-repo-url>
   cd <repository-name>
