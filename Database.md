#                     **Database**         

## &nbsp;

## 1.What do you understand By Database 



### ans:-A database is an organized collection of data that is stored and managed in such a way that it can be easily accessed, managed, and updated. In simpler terms, it’s a system where information is stored systematically for quick retrieval and manipulation.



### 1.Purpose:

### 

* ### To store large amounts of information efficiently.

### 

* ### To allow multiple users or applications to access and modify the data safely.

### 

### 2.Characteristics of a Database:

### 

* ### Structured: Data is stored in a structured way, often in tables (rows and columns).

### 

* ### Persistent: Data is stored permanently until deleted.

### 

* ### Accessible: Data can be retrieved quickly using queries.

### 

* ### Consistent \& Reliable: Ensures accuracy and avoids duplication or corruption.

### 

### 3.Examples of Databases:

### 

* ### Relational Databases (RDBMS): MySQL, Oracle, SQL Server.

### 

* ### NoSQL Databases: MongoDB, Cassandra.

### 

* ### Flat-file Databases: CSV or Excel files.

### 

### 4.Common Uses:

### 

* ### Banking systems to store account information.

### 

* ### E-commerce sites to manage product catalogs and orders.

### 

* ### Social media platforms to store user profiles and posts.









### 2.What is Normalization?

### ans:-

* ### Purpose of Normalization

### 

### 1.Eliminate redundant data: Avoid storing the same data in multiple places.

### 

### 2.Ensure data integrity: Changes or updates happen in only one place, preventing inconsistency.

### 

### 3.Simplify database structure: Makes queries and maintenance easier.

### 

* ### How Normalization Works

### 

### Normalization is done in stages called Normal Forms (NF):

### 

### 1.First Normal Form (1NF):

### 

* ### Each column contains atomic values (no lists or arrays).

### 

* ### Each row is unique.

### 

### 2.Second Normal Form (2NF):

### 

* ### Already in 1NF.

### 

* ### All non-key columns are fully dependent on the primary key (no partial dependency).

### 

### 3.Third Normal Form (3NF):

### 

* ### Already in 2NF.

### 

* ### No transitive dependency 

### 

### 4.Boyce-Codd Normal Form (BCNF) and higher forms exist for more complex scenarios.







### 3.What is Difference between DBMS and RDBMS? 

### ans:-          

### \* **DBMS** (**Database** **Management** **System**):

* #### A software system that allows you to store, manage, and retrieve data.
* #### Can store data as files, hierarchical structures, or other formats.
* #### Limited or no support for relationships between data.
* #### Usually does not enforce normalization.
* #### Less emphasis on data integrity and constraints.
* #### Suitable for small applications.
* #### File system, Microsoft Access, XML databases.



### **\* RDBMS (Relational Database Management System):**

* #### A type of DBMS that stores data in tables (rows and columns) and uses relationships between tables.
* #### Data is always stored in tables with defined relationships.
* #### Supports relationships (primary key, foreign key) between tables.
* #### Supports normalization to reduce redundancy.
* #### Ensures data integrity through constraints like primary key, foreign key, unique key.
* #### Suitable for large-scale applications with multiple users.
* #### MySQL, Oracle, SQL Server, PostgreSQL.









### 4.What is MF Cod Rule of RDBMS Systems?



#### ans:-Rule 1 – Information Rule:

#### 

* #### All information is stored in tables (relations), in rows and columns.

#### 

#### Rule 2 – Guaranteed Access Rule:

#### 

* #### Every piece of data can be accessed using table name, primary key, and column name.

#### 

#### Rule 3 – Systematic Treatment of NULLs:

#### 

* #### Nulls are used to represent missing or inapplicable information, independently of data type.

#### 

#### Rule 4 – Dynamic Online Catalog:

#### 

* #### Database metadata (schema) should be stored in tables, just like user data, and accessible via queries.

#### 

#### Rule 5 – Comprehensive Data Sub-language Rule:

#### 

* #### There should be a single language (like SQL) to handle queries, updates, and transactions.

#### 

#### Rule 6 – View Updating Rule:

#### 

* #### All views (virtual tables) that can theoretically be updated should be updatable through the system.

#### 

#### Rule 7 – High-Level Insert, Update, Delete:

#### 

* #### The system should support set-based operations, not just row-by-row changes.

#### 

#### Rule 8 – Physical Data Independence:

#### 

* #### Changes to physical storage should not affect application programs.

#### 

#### Rule 9 – Logical Data Independence:

#### 

* #### Changes to the logical structure (like adding a column) should not affect application programs.

#### 

#### Rule 10 – Integrity Independence:

#### 

* #### Integrity constraints (like primary keys, foreign keys) are stored in the catalog, not in application code.

#### 

#### Rule 11 – Distribution Independence:

#### 

* #### Users should not need to know if data is distributed across multiple locations.

#### 

#### Rule 12 – Non-subversion Rule:

#### 

* #### If a low-level access method exists, it should not bypass integrity rules.







### 5\. What do you understand By Data Redundancy? 



#### ans:-

#### 1.Definition:

#### 

* #### When the same data is duplicated in different tables or files, it is called data redundancy.

#### 

#### 2.Problems Caused by Data Redundancy:

#### 

* #### Wasted storage space: More memory is used to store duplicate data.

#### 

* #### Data inconsistency: If one copy is updated and others are not, conflicting information arises.

#### 

* #### Difficult maintenance: Updating, deleting, or modifying data becomes more complex.









### 6.What is DDL Interpreter? 



#### ans:-

#### 1.What is DDL?

* #### DDL (Data Definition Language) consists of SQL commands used to define or modify the structure of database objects.

#### Common DDL commands include:

#### 

* #### CREATE – to create tables, databases, or indexes.

#### 

* #### ALTER – to modify the structure of existing tables.

#### 

* #### DROP – to delete tables or databases.

#### 

* #### TRUNCATE – to remove all records from a table but keep its structure.





#### 2\.Role of DDL Interpreter

#### 

* #### The DDL Interpreter takes the DDL statements written by the user.

#### 

* #### It parses these statements to check for syntax errors.

#### 

* #### It translates them into a format the DBMS can understand.

#### 

* #### It updates the system catalog (data dictionary) to reflect changes in the database structure.







### 7.What is DML Compiler in SQL?



#### ans:-

#### 1.What is DML?

#### DML (Data Manipulation Language) consists of SQL commands used to manipulate data in the database.

#### 

#### Common DML commands include:

#### 

* #### INSERT – add new records to a table.
* #### UPDATE – modify existing records.
* #### DELETE – remove records.
* #### SELECT – retrieve data from tables.

#### 

#### 2\. Role of DML Compiler

* #### The DML Compiler takes the DML statements written by the user.
* #### It checks the syntax of the statement.
* #### It translates the statement into low-level instructions that the database can execute.
* #### It interacts with the query processor and storage manager to perform the operations on the actual data.







### 8.What is SQL Key Constraints writing an Example of SQL Key 

### Constraints .



#### ans:-

#### \* Purpose                                                      



* #### Uniquely identifies each row in a table.
* #### Ensures a column’s values match values in another table’s primary key (maintains relationships).
* #### Ensures all values in a column are unique (can be applied to non-primary key columns).
* #### Ensures a column cannot have NULL values.
* #### Ensures a column’s value satisfies a condition.
* #### Provides a default value if none is supplied.



#### 

#### \* Example



* #### StudentID INT PRIMARY KEY
* #### CourseID INT, FOREIGN KEY (CourseID) REFERENCES Courses(CourseID)
* #### Email VARCHAR(50) UNIQUE
* #### StudentName VARCHAR(50) NOT NULL
* #### Age INT CHECK (Age >= 18)
* #### Status VARCHAR(10) DEFAULT 'Active'







### 9.What is save Point? How to create a save Point 

### write a Query?





#### ans:-A Savepoint in SQL is a point within a transaction that allows you to partially commit or rollback the transaction instead of rolling back the entire transaction. It is useful when you want to undo only a part of the transaction without affecting previous operations.





#### \* Key Points About Savepoint



* #### A savepoint marks a point in a transaction.



* #### You can rollback to a savepoint if something goes wrong, instead of rolling back the whole transaction.



* #### Savepoints are used within transactions (BEGIN TRANSACTION ... COMMIT/ROLLBACK).

#### 



### 10.What is trigger and how to create 

### a Trigger in SQL? 



#### ans:-A Trigger in SQL is a special type of stored procedure that is automatically executed  by the database in response to certain events on a table or view.



#### 1.Automatic Execution: Triggers run automatically when a specified event occurs (INSERT, UPDATE, DELETE).



#### 2.Event-Driven: They are associated with table operations.



#### 3.Purpose:



* #### Enforce business rules automatically.



* #### Maintain audit trails (track changes).



* #### Prevent invalid transactions.























