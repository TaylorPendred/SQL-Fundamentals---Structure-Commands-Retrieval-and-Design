# SQL-Fundamentals---Structure-Commands-Retrieval-and-Design
Building a school database in SQLite (In Jupyter Notebook) to practice core SQL. Create/manage tables with correct data types, insert/update/delete records, and run queries for retrieval, filtering, sorting, NULL handling, and aggregates (COUNT, GROUP BY, DISTINCT) to understand relational structure and design principles.

Tasks and Requirements (Answers demonstrated in Notebook File):

-Create a new Google Colab notebook

-Import sqlite3

-Create/connect to an SQLite database

-Create table: StudentTBL (StudentID, FirstName, LastName)

-Create table: Teachers (TeacherID, FirstName, LastName, Subject)

-Create table: Classes (ClassID, ClassName, RoomNumber, TeacherID)

Insert at least 2 students into StudentTBL (e.g., ID 1 John Doe)

Insert at least 2 teachers into Teachers

Insert at least 2 classes into Classes

-Ensure each Classes.TeacherID matches an existing teacher in Teachers

-Select and print all rows from StudentTBL

-Select and print all rows from Teachers

-Select and print all rows from Classes

-Query Classes where TeacherID = 1 OR RoomNumber = 12, order by ClassName ASC

-Query StudentTBL for FirstName + LastName where StudentID IN (1, 3, 5)

-Update one class in Classes and set RoomNumber = NULL

-Query Classes where RoomNumber IS NULL
-Query first 2 students from StudentTBL ordered by LastName ASC (use LIMIT 2)
-Count total classes in Classes where TeacherID = 2
-Count classes per TeacherID in Classes (GROUP BY TeacherID) and order by count ASC
-Count distinct room numbers used in Classes (COUNT(DISTINCT RoomNumber))
-Alter Classes to add column Semester
-Update all Classes rows to set Semester = 'Semester 2'
-Delete from Classes where RoomNumber = 10
