# SQL
All about Sequel


## Data types
* **INT**: _Whole numbers_
* **FLOAT (M,D)**: _Decimal numbers (approximate) ie rounding_
* **DECIMAL (M,D)**: _Decimal numbers (precise) ie price_ - DECIMAL(3,2) means that the entire number at the end should have 3 visible digits of which two are decimals.
* **CHAR (N)**: _Fixed lenght Character_
* **VARCHAR (N)**: _Varying lenght character_
* **ENUM ('M','F')**: _Value from a defined list_
* **BOOLEAN**: _True or False values_
* **DATE**: _Date (YYYY-MM-DD)_
* **DATETIME**: _Date and the time (YYYY-MM-DD HH-MM-SS)_
* **TIME**: _Time (HHH-MM-SS)_
* **YEAR**: _Year (YYYY)_


## Primary key and foreign key

* A primary key is a column which uniquely identifies a record within a table
* It cannot be null

* A foreign key is a column whose values match the values of another tables primary key column
* The table with the primary key is called the reference, or parent table 
* The table with the foreign key is called the child table.
* A table can have multipile foreign keys


## `SHOW DATABASES`:
- Shows all existing databases in that database management system

## `CREATE DATABASE _databaseName_`:
- This code creates a new database

## `USE _databaseName_`:
- Allows you to edit an existing database

## `CREATE TABLE _tableName_();`:
- Creates a new table within the database in use

```
 CREATE TABLE products(
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(30)
    price DECIMAL(3,2)
 );
```

## `SHOW TABLES;`:
- Returns a list of available tables

## Creating foreign keys:
```
CREATE TABLE orders(
  id INT AUTO_INCREMENT PRIMARY KEY,
  product_id INT,
  customer_id INT,
  order_time DATETIME,
  FOREIGN KEY (product_id) REFERENCES products(id),
  FOREIGN KEY (customer_id) REFERENCES customers(id)
);
```
