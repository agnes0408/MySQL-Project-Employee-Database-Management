Create Database employee ;

-- Use the database
use employee ;

-- Create Departments table
CREATE TABLE departments (
    department_id INT ,
    department_name VARCHAR(100)
);

-- Create Location table
CREATE TABLE location (
    location_id INT ,
    location VARCHAR(30)
);

 -- Create Employees table
 CREATE TABLE employees (
    employee_id INT ,
    employee_name VARCHAR(50),
    gender ENUM('M', 'F'),
    age INT,
    hire_date DATE,
    designation VARCHAR(100),
    department_id INT,
    location_id INT,
    salary DECIMAL(10,2),
);
    
    
 -- Add a new column "email"
ALTER TABLE employees
ADD COLUMN email VARCHAR(100);

-- Modify "designation" to support wider range (increase length)
ALTER TABLE employees
MODIFY COLUMN designation VARCHAR(200);

-- Drop the "age" column
ALTER TABLE employees
DROP COLUMN age;

-- Rename "hire_date" to "date_of_joining"
ALTER TABLE employees
CHANGE COLUMN hire_date date_of_joining DATE;
   
   -- Rename "Departments" to "Departments_Info"
RENAME TABLE departments TO departments_info;

-- Rename "Location" to "Locations"
RENAME TABLE location TO locations;

    -- Truncate the Employees table
TRUNCATE TABLE employees;

-- Drop the Employees table
DROP TABLE employees;

-- Drop the employee database
DROP DATABASE employee;


-- Drop the database if it exists
DROP DATABASE IF EXISTS employee;

-- Recreate the database
CREATE DATABASE employee;

-- Use the recreated database
USE employee;

CREATE TABLE departments (
    department_id INT PRIMARY KEY,  
    department_name VARCHAR(100) NOT NULL UNIQUE  
);

CREATE TABLE location (
    location_id INT AUTO_INCREMENT PRIMARY KEY,  
    location VARCHAR(30) NOT NULL UNIQUE  
);

CREATE TABLE employees (
    employee_id INT PRIMARY KEY,
    employee_name VARCHAR(50) NOT NULL,
    gender ENUM('M', 'F') NOT NULL,
    age INT CHECK (age >= 18),
    hire_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    designation VARCHAR(200),
    department_id INT,
    location_id INT,
    salary DECIMAL(10,2),
    email VARCHAR(100),
    FOREIGN KEY (department_id) REFERENCES departments(department_id),
    FOREIGN KEY (location_id) REFERENCES location(location_id)
);






    
    
    
    
    
    
    
    
