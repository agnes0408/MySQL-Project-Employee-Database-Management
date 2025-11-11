
MySQL Project – Employee Database Management
📘 Overview

This project demonstrates the creation and management of an Employee Database using MySQL.
It covers key database concepts such as DDL commands, constraints, and querying data, simulating a real-world HR and department management system.

🧩 Project Structure
📂 Employee_Database_Project
├── 📄 MySQL_Assignment_1_DDL_Commands.sql
├── 📄 MySQL_Assignment_2_Querying_Data.sql
├── 📄 Employee_Data_Insert.sql
├── 📘 README.md

⚙️ Assignment 1 – DDL Commands & Constraints
🏗️ Database & Tables:

Created a database named employee and the following tables:

Departments

Location

Employees

🔧 DDL Operations:

CREATE – Defined tables with primary keys, foreign keys, and constraints.

ALTER –

Added column email to Employees

Modified designation data type

Dropped age column

Renamed hire_date → date_of_joining

RENAME – Renamed Departments → Departments_Info, and Location → Locations.

TRUNCATE & DROP – Used to clear and remove tables/databases when needed.

🔒 Constraints:

Unique Identifiers for department_id and employee_id.

NOT NULL and UNIQUE applied to names and location fields.

CHECK Constraints:

Gender limited to ‘M’ or ‘F’.

Minimum age = 18.

DEFAULT – date_of_joining auto-fills with the current date.

FOREIGN KEYS – Linked employees to departments and locations.

📊 Assignment 2 – Querying Data
🔍 Data Retrieval & Filtering:

DISTINCT: Extracted unique salary values.

ALIAS: Renamed columns (Employee_Age, Employee_Salary).

WHERE: Filtered employees with salary > ₹50,000 and hired before 2016.

UPDATE: Filled missing designations with “Data Scientist”.

🔢 Sorting & Grouping:

ORDER BY: Sorted employees by department & salary.

LIMIT: Displayed first 5 employees from 2018.

AGGREGATES: Calculated total salary, minimum age, and average salary.

GROUP BY: Aggregated salaries and averages per department/designation.

HAVING: Filtered departments and locations based on employee count & average age.

🔗 Joins:

INNER JOIN: Linked employees with departments.

LEFT JOIN: Displayed all departments with employee counts.

RIGHT JOIN: Showed all locations with or without assigned employees.

📈 Outcome

✅ Built a robust relational database for managing employee, department, and location data.
✅ Practiced real-world SQL operations including DDL, DML, Joins, and Constraints.
✅ Strengthened understanding of database design, normalization, and query optimization.

🧰 Tools Used

MySQL Workbench

SQL Editor / Command Line

ERD Modeling

🧑‍💻 Author

Developed by Agnes A
A hands-on SQL project demonstrating database creation, manipulation, and analysis.
