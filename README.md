Employee Database Management System (EDMS)
A Java-based application for managing employee records using JDBC (Java Database Connectivity) to interact with an SQL database. This system provides efficient operations for adding, updating, deleting, and retrieving employee data from a database.

Features
Add Employees: Add new employee records to the database.
Update Employees: Modify existing employee details.
Delete Employees: Remove employee records using their ID.
Search Employees: Retrieve employee details by ID.
Display All Employees: List all employees in the database.

Technologies Used
Java: Core programming language.
JDBC: For database connectivity.
SQL: To manage employee data in the database (MySQL/PostgreSQL/SQLite).
Database Driver: MySQL Connector/J or other compatible drivers.

Setup and Installation

1. <b>Clone the Repository</b>

       git clone https://github.com/your-username/employee-database-management.git  
       cd employee-database-management  
3.  <b>Set Up the Database</b>   
    Create a database
                  
         CREATE DATABASE EmployeeDB;
    Create a table for employees:

        CREATE TABLE Employee (
        id INT PRIMARY KEY,
        name VARCHAR(100),
        department VARCHAR(50),
        salary DOUBLE
        );
 3. <b>Configure Database Connection</b>
    Update the database credentials in the DBConnection.java file:

        private static final String URL = "jdbc:mysql://localhost:3306/EmployeeDB";
        private static final String USER = "your_username";
        private static final String PASSWORD = "your_password";
4. Compile and Run the Project  
     Compile all Java files

         javac *.java
     Run the main class

         java Main
   <b>How It Works</b><br>
    ->The program connects to the SQL database using JDBC.<br>
    ->Employee records are stored and managed in the SQL table.<br>
    ->Operations like adding, updating, deleting, and searching are performed using SQL queries.<br>

<br>
<br>
<b>Project Structure</b><br>
  
    ├── Employee.java          # Employee data class
    ├── DBConnection.java      # Manages the database connection
    ├── EmployeeOperations.java # Contains CRUD methods
    ├── Main.java              # Entry point to the application

  

     
   

