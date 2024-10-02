# SQL Documentation: Basic SQL Commands

This documentation provides an overview of essential SQL commands, enabling users to perform key database operations such as displaying, creating, deleting, selecting, and inserting data. Each command includes the purpose, syntax, and examples for clarity.

---

## 1. SHOW

### Purpose
The `SHOW` command displays information about databases, tables, or columns within a table.

### Syntax

```sql
SHOW {DATABASES | TABLES | COLUMNS FROM table_name};
```

### Examples

- **Display all databases:**

    ```sql
    SHOW DATABASES;
    ```

- **Display all tables in the current database:**

    ```sql
    SHOW TABLES;
    ```

- **Display columns of a specific table:**

    ```sql
    SHOW COLUMNS FROM employees;
    ```

---

## 2. CREATE

### Purpose
The `CREATE` command is used to create a new database or table.

### Syntax

- **Create a database:**

    ```sql
    CREATE DATABASE database_name;
    ```

- **Create a table:**

    ```sql
    CREATE TABLE table_name (
        column1_name data_type constraints,
        column2_name data_type constraints,
        ...
    );
    ```

### Examples

- **Create a new database:**

    ```sql
    CREATE DATABASE my_database;
    ```

- **Create a new table:**

    ```sql
    CREATE TABLE employees (
        id INT PRIMARY KEY,
        name VARCHAR(50),
        position VARCHAR(50),
        salary DECIMAL(10, 2)
    );
    ```

---

## 3. DROP

### Purpose
The `DROP` command deletes a database or table permanently.

### Syntax

- **Drop a database:**

    ```sql
    DROP DATABASE database_name;
    ```

- **Drop a table:**

    ```sql
    DROP TABLE table_name;
    ```

### Examples

- **Drop a database:**

    ```sql
    DROP DATABASE my_database;
    ```

- **Drop a table:**

    ```sql
    DROP TABLE employees;
    ```

---

## 4. SELECT

### Purpose
The `SELECT` command retrieves data from a database.

### Syntax

```sql
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

### Examples

- **Select all columns from a table:**

    ```sql
    SELECT * FROM employees;
    ```

- **Select specific columns from a table:**

    ```sql
    SELECT name, position FROM employees;
    ```

- **Select data with a condition:**

    ```sql
    SELECT name, salary
    FROM employees
    WHERE position = 'Manager';
    ```

---

## 5. INSERT

### Purpose
The `INSERT` command adds new rows to a table.

### Syntax

```sql
INSERT INTO table_name (column1, column2, ...)
VALUES (value1, value2, ...);
```

### Examples

- **Insert a single row into a table:**

    ```sql
    INSERT INTO employees (id, name, position, salary)
    VALUES (1, 'Samuel Davies', 'CEO', 80000.00);
    ```

- **Insert multiple rows into a table:**

    ```sql
    INSERT INTO employees (id, name, position, salary)
    VALUES
    (2, 'Henry Davies', 'App Support', 65000.00),
    (3, 'Emily Johnson', 'Product Designer', 60000.00);
    ```

---

## Conclusion

These basic SQL commands—`SHOW`, `CREATE`, `DROP`, `SELECT`, and `INSERT`—are essential for managing and interacting with relational databases. Mastery of these commands will enable users to perform a variety of database operations effectively.
