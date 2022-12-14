# SQL
All about Sequel


## Data types
* **INT**: _Whole numbers_
* **FLOAT (M,D)**: _Decimal numbers (approximate) ie rounding_
* **DECIMAL (M,D)**: _Decimal numbers (precise) ie price_
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
