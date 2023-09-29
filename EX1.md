# EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS

## AIM:
To create a student database and execute DDL queries using SQL.


## DDL (Data Definition Language)
<div align="justify">
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
</div>
 
## List of DDL commands: 
<div align="justify">
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.
</div>

## Query:
### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.

### SQL QUERY: 
```
CREATE TABLE student(
    rollno numeric(5),name char(50),age numeric(5),
    address varchar(100),
    phoneno numeric(10)
    );
```
### OUTPUT:

![image](https://github.com/MIRUDHULA-DHANARAJ/G2_DBMS/assets/94828147/a0ddd93d-ee20-467c-bc16-09b150f263fe)


### 2) Change the above student table by adding another attribute department

### SQL QUERY: 
```
ALTER TABLE student ADD Department char(10);
```
### OUTPUT:

![image](https://github.com/MIRUDHULA-DHANARAJ/G2_DBMS/assets/94828147/3a0c11dd-f0a7-4e73-80cc-41ce502f509a)


### 3) Drop the student table
 
### SQL QUERY: 
```
DROP TABLE student;
```
### OUTPUT:

![image](https://github.com/MIRUDHULA-DHANARAJ/G2_DBMS/assets/94828147/5536abfd-143c-4dff-b293-d13f918a2d6e)


### 4) Delete the student table using truncate keyword

### SQL QUERY: 
```
TRUNCATE TABLE student;
```
### OUTPUT:

![image](https://github.com/MIRUDHULA-DHANARAJ/G2_DBMS/assets/94828147/c5f14c5f-c6f7-4f7d-9aca-5414b1bc1058)


### 5) Rename the student table to mystudent

### SQL QUERY: 
```
ALTER TABLE student RENAME TO mystudent;
```
### OUTPUT:

![image](https://github.com/MIRUDHULA-DHANARAJ/G2_DBMS/assets/94828147/82c85dcb-7e3b-4d03-9b77-ad48e6d00064)

### RESULT:
Thus a student database has been created and DDL queries are executed successfully.
