SQL 1: Intro to DBMS and Relational Model

**SQL (Structured Query language)**
MongoDB is a NoSQL Data Base

DBMS => Data Base Management System

Data base allows you to do CRUD operations => Create, Read Update & Delete

SQL is a query language

Data base is the collection of Data, & the system that alows you to put data, fetch Data is called DBMS

SQL is a language through which you do CRUD

Data Base has 2 types:

1. Relational Database = which has tables and we can manage the Data tye in coloumns, & collection of rows & coloumns is called a table example: Excel sheet, like in a Excel sheet we can refer to as a table, and collection of tables is called a Database (table is a collection of rows & coloumns & collection of tables if called a relational database)
     Each coloumn should have a type & no 2 rows should be identical, & value should be atomic in a row + coloumn => Atomic (lets say if any user has multiple phone number then it should be stored in different-2 coloumns that would be good practice)
2. NoSQL Database 

**Candidate key:** is the minimum set of coloums required which is guranteed to be unique, like {email, EmployeeId}, both can be candidate key seprately , and super key can be combined of {email, EmployeeId}

In a given table we can have multiple candidate keys, like in a student table, Id, email & phone Number are candidate keys

one of the candidate key in a table, it is chosen as a primary key
we can apply binary search tree using id, says every smaller id is on the left side & every larger entry is on right side so we can find it in O(Log N) Time
so we dont want to make a coloumn which gets changes very often, like if a person changes their phone number, then it cant be optimized to use these coloumns as primary key
**Foreign Key:** it only applicaple when we have 2 tables and there is some connection in between them.
if there is entry which is unique, & if i want to havw another table and there is some connection & one tablw is referring to have some id, & every entry in Table 1 for id have some connection corresponds to unique row in another table, When that kind of relation is established that is called as a Foreign key & thus we cant have any randon id, if that id is not present in another table, & if we delete entry in a table and there is foreign key relationship then it will delete that row in another table as well, & if there is foreign key relationship then we neither be able to create any random id row & deletion via foreign key in another table is also called cascading delete.
**Cascading deletion:** if one entry is deleted and it has foreign key relationship in Database, then all entries in all tables with that id are deleted.












