# Northwind.sql

# SQL Database for Practice & Learning

This repository contains the W3Schools SQL database, cleaned and formatted for use in [DB Fiddle](https://www.db-fiddle.com/) (MySQL 8.0). It includes 8 tables: `Categories`, `Customers`, `Employees`, `Orders`, `OrderDetails`, `Products`, `Shippers`, and `Suppliers`. The data is ideal for practicing SQL queries.

## Table Structure
- **Categories**: 8 records (product categories)
- **Customers**: 91 records (customer details)
- **Employees**: 10 records (employee details)
- **Orders**: 401 records (customer orders)
- **OrderDetails**: 518 records (order items)
- **Products**: 77 records (product details)
- **Shippers**: 3 records (shipping companies)
- **Suppliers**: 29 records (product suppliers)

## How to Use
1. Go to [DB Fiddle](https://www.db-fiddle.com/).
2. Select **MySQL 8.0** as the database engine.
3. Copy the SQL code from one of the `.sql` files (e.g., `customers.sql`) or use `w3schools_full.sql` for the entire database.
4. Paste the code into the **Schema** panel (left side).
5. Click **Run** to create the tables and insert data.
6. Write and test your SQL queries in the **Query** panel (right side).
7. Save or share your fiddle using the provided URL.

**Note**: Insert tables in dependency order (`Categories`, `Suppliers`, `Products`, `Customers`, `Employees`, `Shippers`, `Orders`, `OrderDetails`) to avoid foreign key errors.

## Files
- `Categories.sql`: Schema and data for `Categories` table.
- `Customers.sql`: Schema and data for `Customers` table.
- `Employees.sql`: Schema and data for `Employees` table.
- `Orders.sql`: Schema and data for `Orders` table.
- `OrderDetails.sql`: Schema and data for `OrderDetails` table.
- `Products.sql`: Schema and data for `Products` table.
- `Shippers.sql`: Schema and data for `Shippers` table.
- `Suppliers.sql`: Schema and data for `Suppliers` table.
- `ConcatentedData.sql`: Combined schema and data for all tables.

## Cleaning Applied
- Set NULL `PostalCode` in `Customers` to 'Unknown'.
- Removed spaces from `PostalCode` in `Customers` and `Suppliers`.
- Normalized `Phone` formats in `Suppliers` and `Shippers` (e.g., '(503) 555-9831' → '503-555-9831').
- Rounded `Price` in `Products` to 2 decimal places.

## Tips
- If DB Fiddle is slow, use individual table files or a subset of the data.
- For local testing, import the `.sql` files into MySQL Workbench or a similar tool.
- Practice queries like `SELECT`, `JOIN`, `GROUP BY`, and `SUBQUERY` using this dataset.

## License
This dataset is provided for educational purposes. Feel free to use and share it for teaching SQL.
