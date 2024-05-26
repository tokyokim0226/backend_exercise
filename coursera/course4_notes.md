# Course 4 - Databases

#### Database
- A form of electronic storage that holds data
- [Course Goals](https://www.coursera.org/learn/intro-to-databases-back-end-development/supplement/TptnH/course-syllabus-introduction-to-databases)
-  each instance must be uniquely identifiable
-  **Primary Key Field** - unique values that cannot be replicated elsewhere in the table/entity
   - This avoids potential confusion between tables with similarities in data
 - **Foreign Key** - a field in one table that connects to the primary key field in the original table
 - **Big data** - complex data that grows exponentially with time

#### Stages of Databases (History)
**Flat Files**
- Used during 1970s-1990s
- A type of a database system that stores data in a single file or table - basically text files, where every line contains one record and fields either have fixed lengths or are separated by commas, whitespaces, and tabs - cannot contain multiple tables
(Think of an excel file in CSV format)

**Hierarchical database systems**
- store data in a hierarchically arranged manner
- One to many relationship - parent can have multiple children, but one child can only have one parent

**Network databases**
- unlike the hierarchical database model, allows multiple parent child relationships - many to many relationships (memberse & owners)
- has a graph-like structure

**Relational Database system**
- Data is stored in tables
- Columns of the table hold attributes of the data
- Each record usually has a value for each attribute
- In a relational database, each row in the table is a record with a unique ID attribute called the primary key
- A relational database stores and provides access to data that are related to one anotehr using an ttribute known as a foreign key
  - Foreign keys can be duplicate/null as they serve to show the relation between databases/tables

**Object Oriented Databases**
- these are databases that store data in the form of objects as opposed to the traditional relational databases that store data in tables
- Data is encapsulated within objects, which can contain attribtues (data fields) and methods (functions or precedures taht operate on the data).
- These objects are instances of classes, which define the structure and behavior of the objects


**NoSQL databases**
- Preferred over relational databases because relational databases only allows to store structured data.
- NoSQL databases are faster and more flexible in storing data - can deal with unstructured data
- Data can be stored in an ad-hoc manner and they allow to store and process high volumes of different kinds of data

### Structured Query Langauge (SQL)

**CRUD operations** - Create, Read, Update, Delete

**SQL** - Standard language that can interact with structured data on databases
- Used to communicate with and manipulate databases
- Used for querying, updating, and managing data in relational database management systems 
- Some key functions include SELECT, INSERT, UPDATE, DELETE, CREATE, ALTER, DROP, GRAND, REVOKE, etc.
**MySQL** - A specific relational database management system that uses SQL as its query language

- SQL is like English (a language), while MySQL is like a specific book written in English. Many books can be written in English, just like there are many RDBMS (relational database management system) systems that use SQL

#### SQL Subsets

SQL consists of several subsets, each designed for different types of database operations. These subsets help categorize the various functionalities of SQL, making it easier to understand and use. The main subsets of SQL are:
1. **Data Definition Language (DDL)** - defines and manages database structures
   1. CREATE, ALTER, DROP, TRUNCATE, RENAME
2. **Data Manipulation Language** - Manages data within the database
   1. SELECT, INSERT, UPDATE, DELETE
3. **Data Control Language** - Controls access to the data
   1. GRANT, REVOKE
4. **Transaction Control Language** - Manages transactions to ensure data integrity
      1. COMMIT, ROLLBACK, SAVEPOINT, RELEASE SAVEPOINT, SET TRANSACTION