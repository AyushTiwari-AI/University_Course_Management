University Course Management System
Project
SQL Final Project — University Course Management System.
Objective
Create a database for a university using SQL. The database stores students, courses, instructors, enrollments, and departments and demonstrates CRUD operations, joins, filtering, aggregation, subqueries, string/date functions, CASE, and a window function.
Tables
1. Students — StudentID, FirstName, LastName, Email, BirthDate, EnrollmentDate
2. Courses — CourseID, CourseName, DepartmentID, Credits
3. Instructors — InstructorID, FirstName, LastName, Email, DepartmentID, Salary
4. Enrollments — EnrollmentID, StudentID, CourseID, EnrollmentDate
5. Departments — DepartmentID, DepartmentName
Requirements
- MySQL 8.0 or later (the project uses LIMIT, YEAR(), CONCAT(), DATE_SUB(), and a window function).
- MySQL Workbench or another MySQL client.
How to Run
1. Open MySQL Workbench and connect to your MySQL server.
2. Open University_Course_Management.sql.
3. Execute the script.
4. The script creates the database and tables, inserts the assignment's sample data, and runs all 16 queries.
5. Read the result grid after each SELECT query.
Queries Included
1. CRUD operations for all tables.
2. Students who enrolled after 2022.
3. Mathematics department courses, limited to 5.
4. Courses with more than 5 enrolled students.
5. Students enrolled in both Introduction to SQL and Data Structures.
6. Students enrolled in either Introduction to SQL or Data Structures.
7. Average credits of all courses.
8. Maximum instructor salary in Computer Science.
9. Number of students enrolled in each department.
10. INNER JOIN of students and their courses.
11. LEFT JOIN to show all students and any courses.
12. Students in courses with more than 10 students.
13. Extract enrollment year.
14. Concatenate instructor first and last names.
15. Running total of course enrollments.
16. Senior/Junior label based on enrollment date.
Assumption
The assignment's Instructors field list does not include Salary, but Query 8 asks for maximum instructor salary. To make that query executable, a Salary column was added to the Instructors table and sample salary values were assumed. Update these sample values if your instructor provides specific salaries.
Notes
- The script uses only the two sample students and two sample courses shown in the assignment. Therefore, queries requiring more than 5 or more than 10 students may return no rows with the supplied sample data. This is expected.
- UPDATE and DELETE examples are commented out so the original sample data is not changed accidentally. Uncomment and run an example only when needed.
- Keep the SQL code original and make sure you understand the queries before submitting.
