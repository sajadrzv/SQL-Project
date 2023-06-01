# SQL-Project
Developing a Database for University Library
Designing a database with MySQL for university library including the relations and inserted records.
This project is about designing database of a university library. This database gives information regarding the books, authors, publishers, and the students that borrow these books. 
•	A book can be authored at the most by many authors and at the least by one author. An author at the most can author many books and at the least can author one book. So, the relation between two tables of Author and Book is many-to-many. This is why we need a bridge table that the primary key of Author and Book tables are its foreign keys. 
•	A book can at the most be published by one publisher and at the least be published by one publisher (meaning, a book is published by exactly one publisher). A publisher can publish at the most many books and at the least one book. So, the relationship between publisher and book is One-to-Many and the primary key of Publisher is the foreign key in Book.
•	A student at the most can borrow many books and at the least zero books (this is because some students never borrow books). A book at the most is borrowed by one student and at the least by one student (meaning, a book is borrowed by exactly one student). So, the relationship between Student and Book is One-to-Many and Student Primary key is the foreign key in Book Table. And the Min Cardinality is One-to-Zero
•	An employee can at the most borrow one book and at the least zero books (this is because some employees never borrow books). A book at the most is borrowed by one employee and at the least by one employee (meaning, a book is borrowed by exactly one employee).So, the Max Cardinality between Employee and Book Tables is One-to-One. For this also, we consider the PK of Employee to be FK on Book table.

Then we start creating tables, and their constraint.
