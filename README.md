Week 2 Assignment: Introduction to SQL
Assignment Overview

This assignment focuses on the fundamentals of SQL (Structured Query Language). It demonstrates how to retrieve and manipulate data from a relational database using basic SQL queries.

The assignment uses the sales database and covers selecting columns, filtering records, sorting results, and limiting query outputs.

Database Used
Database Name: sales
Database Management System: MySQL
Tables Used:
payments
orders
employees
offices
products
Database Setup

Before running the queries, ensure that the sales database is installed and available in MySQL.

To display the available databases, run:

sql
SHOW DATABASES;


To select the sales database, run:

sql
USE sales;

Assignment Questions and Solutions
Question 1: Retrieve Payment Information

Objective: Retrieve the check number, payment date, and amount from the payments table.

SQL Query:

sql
SELECT checkNumber, paymentDate, amount
FROM payments;


Concepts Used:

SELECT
FROM
Question 2: Find Orders in Process

Objective: Retrieve the order date, required date, and status of orders that are currently in process. Sort the results by order date in descending order.

SQL Query:

sql
SELECT orderDate, requiredDate, status
FROM orders
WHERE status = 'In Process'
ORDER BY orderDate DESC;


Concepts Used:

SELECT
FROM
WHERE
ORDER BY
DESC
Question 3: Find Sales Representatives

Objective: Retrieve the first name, last name, and email of employees whose job title is Sales Rep. Sort the results by employee number in descending order.

SQL Query:

sql
SELECT firstName, lastName, email
FROM employees
WHERE jobTitle = 'Sales Rep'
ORDER BY employeeNumber DESC;


Concepts Used:

SELECT
FROM
WHERE
ORDER BY
DESC
Question 4: Retrieve Office Information

Objective: Retrieve all columns and all records from the offices table.

SQL Query:

sql
SELECT *
FROM offices;


Concepts Used:

SELECT
FROM
Wildcard operator (*)
Question 5: Retrieve the Five Cheapest Products

Objective: Retrieve the product name and quantity in stock for the five cheapest products, sorting by purchase price in ascending order.

SQL Query:

sql
SELECT productName, quantityInStock
FROM products
ORDER BY buyPrice ASC
LIMIT 5;


Concepts Used:

SELECT
FROM
ORDER BY
ASC
LIMIT
SQL Concepts Covered
SQL Keyword	Description
SELECT	Retrieves data from a database
FROM	Specifies the table to retrieve data from
WHERE	Filters records based on a condition
ORDER BY	Sorts query results
ASC	Sorts results in ascending order
DESC	Sorts results in descending order
LIMIT	Restricts the number of returned records
*	Retrieves all columns from a table
Tools and Technologies
MySQL
MySQL Workbench (or MySQL Command Line Client)
SQL
How to Run the Assignment
Open MySQL Workbench.
Connect to your MySQL database server.
Confirm that the sales database exists.
Execute USE sales;.
Copy and execute each SQL query.
Review the results displayed in the output panel.
Save your SQL script and capture screenshots of the results.
Learning Outcomes

After completing this assignment, I have practiced how to:

Retrieve specific columns from database tables.
Filter records using the WHERE clause.
Sort records using ORDER BY.
Apply ascending and descending sorting.
Limit query results using LIMIT.
Retrieve all columns and records from a table.
Work with multiple tables in a relational database.
Conclusion

This assignment provided practical experience with fundamental SQL commands using the sales database. It strengthened my understanding of how to retrieve, filter, and organize information stored in relational databases.

These SQL fundamentals provide a foundation for more advanced database operations and data analysis.

**Assignment
