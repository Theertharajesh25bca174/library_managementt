COLLEGE LIBRARY MANAGEMENT SYSTEM
==================================

Project: SQL Section C - Research Project
Course: BCA Data Science
Database: MySQL
Database name: librarydb

FILES
-----
library_project.sql
    Complete SQL script: database creation, tables, sample data,
    questions C2-C12, stored procedure C13 and trigger C14.

ERD.drawio
    Editable Entity Relationship Diagram. Open it using diagrams.net.

ERD.png
    Exported image of the ER diagram (add this after exporting it).

HOW TO RUN
----------
1. Open https://onecompiler.com/mysql or another MySQL 8.0-compatible
   online SQL editor.
2. Open library_project.sql in a text editor.
3. Copy the SQL into the online editor and execute it.
4. If the website limits long scripts or stored procedures/triggers,
   run the script in sections. Use a MySQL 8.0-compatible environment
   for the RANK() window function, stored procedure and trigger.
5. Execute the SELECT statements and check the displayed results.

DATABASE STRUCTURE
------------------
The project contains three tables:

1. members
   Primary key: member_id

2. books
   Primary key: book_id

3. issues
   Primary key: issue_id
   Foreign keys: member_id references members(member_id)
                 book_id references books(book_id)

RELATIONSHIPS
-------------
One member can have many issue records (members 1-to-many issues).
One book can appear in many issue records (books 1-to-many issues).

FINE RULE
---------
Fine = number of late days x Rs. 2.
A NULL return_date means that the book has not yet been returned.

NOTE
----
The SQL file is based on the supplied project schema and sample dataset.
Please run and understand each query before the viva. The trigger is
created on copies of the books and issues tables so that the original
sample tables remain unchanged.

GitHub repository should be public so that the lecturer can open the link
without signing in.
