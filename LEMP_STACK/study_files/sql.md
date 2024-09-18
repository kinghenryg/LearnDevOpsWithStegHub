# Structured Query Language (SQL) Overview

**SQL (Structured Query Language)** is a standardized language designed for managing and manipulating relational databases. It provides a powerful means to perform operations such as creating, retrieving, updating, and deleting data within a database. This document covers the basic syntax of SQL and its most frequently used commands for effective data management.

## Basic SQL Syntax

SQL commands are structured to perform specific actions on database tables. Here are some essential SQL commands:

- **SELECT Statement:** Retrieves data from one or more tables.

    ```sql
    SELECT column1, column2 FROM table_name;
    ```

- **INSERT Statement:** Adds new records to a table.

    ```sql
    INSERT INTO table_name (column1, column2) VALUES (value1, value2);
    ```

- **UPDATE Statement:** Updates existing records in a table.

    ```sql
    UPDATE table_name SET column1 = value1 WHERE condition;
    ```

- **DELETE Statement:** Deletes records from a table.

    ```sql
    DELETE FROM table_name WHERE condition;
    ```

- **CREATE TABLE Statement:** Defines and creates a new table with specified columns and data types.

    ```sql
    CREATE TABLE table_name (
      column1 datatype,
      column2 datatype
    );
    ```

- **ALTER TABLE Statement:** Modifies the structure of an existing table, such as adding or removing columns.

    ```sql
    ALTER TABLE table_name ADD column_name datatype;
    ```

- **DROP TABLE Statement:** Permanently removes a table from the database.

    ```sql
    DROP TABLE table_name;
    ```

## Key SQL Commands

SQL includes several commands for advanced data management and retrieval:

- **SELECT:** Retrieves specific columns or all columns from a table. Results can be filtered using a `WHERE` clause.

    ```sql
    SELECT * FROM employees;
    ```

- **WHERE Clause:** Filters rows based on specific criteria.

    ```sql
    SELECT * FROM employees WHERE department = 'HR';
    ```

- **ORDER BY Clause:** Sorts results by one or more columns in ascending or descending order.

    ```sql
    SELECT * FROM employees ORDER BY salary DESC;
    ```

- **GROUP BY Clause:** Groups rows that have the same values in specified columns to summarize data.

    ```sql
    SELECT department, COUNT(*) FROM employees GROUP BY department;
    ```

- **JOIN Command:** Combines rows from two or more tables based on related columns.

    ```sql
    SELECT e.name, d.name FROM employees e JOIN departments d ON e.department_id = d.id;
    ```

- **COUNT Function:** Counts the number of rows that match a specified condition.

    ```sql
    SELECT COUNT(*) FROM employees;
    ```

- **SUM, AVG, MIN, MAX Functions:** Perform calculations such as summing, averaging, finding minimum, and maximum values.

    ```sql
    SELECT SUM(salary) FROM employees;
    ```

## Example Screenshots

Below are example screenshots illustrating SQL commands and their outputs:

1. **Basic SELECT Query:**
   ![SELECT Query Example](./images/query-table.png)

2. **INSERT INTO Operation:**
   ![INSERT Operation Example](path/to/insert-rows.png)

3. **Table Creation and Structure:**
   ![Table Creation Example](path/to/table-creation.png)

## Conclusion

This overview introduces fundamental SQL syntax and commonly used commands. Mastery of these basics, combined with practice and exploration of more complex queries, will enable you to effectively manage and analyze data using SQL.

For more detailed explanations and advanced SQL topics, refer to [W3Schools SQL Tutorial](https://www.w3schools.com/sql/).
