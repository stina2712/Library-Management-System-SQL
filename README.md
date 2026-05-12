# Library-Management-System-SQL
# [Project Name, e.g., Library Management System]

## 📌 Project Overview
This project demonstrates my ability to design a relational database and write complex SQL queries. I built this to solve the problem of [e.g., tracking book loans and member activity].

## 🛠️ Tech Stack
- **Database:** MySQL / PostgreSQL (Pick one)
- **Tool:** MySQL Workbench / VS Code
- **Language:** SQL

## 📊 Database Schema (ER Diagram)
Below is the structure of the database:
- **Students Table:** Stores IDs, names, and enrollment dates.
- **Courses Table:** Tracks available classes and credit hours.
- **Enrollments Table:** Connects students to their courses.

## 🚀 Key SQL Features Demonstrated
- **Data Definition (DDL):** Creating structured tables with Primary and Foreign keys.
- **Joins:** Combining data from multiple tables to generate reports.
- **Aggregations:** Using `GROUP BY` and `COUNT` to analyze data trends.

## 🔍 Sample Query
Here is an example of a query I wrote to find the most popular course:

\`\`\`sql
SELECT CourseName, COUNT(StudentID) AS Total_Students
FROM Enrollments
JOIN Courses ON Enrollments.CourseID = Courses.CourseID
GROUP BY CourseName
ORDER BY Total_Students DESC;
\`\`\`

## 📂 How to Use
1. Clone this repository.
2. Run `schema.sql` to create the database structure.
3. Run `data.sql` to insert sample records.
4. Execute `queries.sql` to see the analysis in action.
