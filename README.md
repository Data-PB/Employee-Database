# Employee-Database

## Background
Analyze employee data of the corporation from the 1980s and 1990s. All that remain of the database of employees from that period are six CSV files.

## Data Modeling
Inspected the CSVs and sketched out an ERD of the tables. Used a tool like http://www.quickdatabasediagrams.com.

![ERD](ERD.png)

## Data Engineering
* Used the information to create a table schema for each of the six CSV files by specifying data types, primary keys, foreign keys, and other constraints.
* Imported each CSV file into the corresponding SQL table.

## Data Analysis
1.	Listed the following details of each employee: employee number, last name, first name, gender, and salary.
2.	Listed employees who were hired in 1986.
3.	Listed the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name, and start and end employment dates.
4.	Listed the department of each employee with the following information: employee number, last name, first name, and department name.
5.	Listed all employees whose first name is "Hercules" and last names begin with "B."
6.	Listed all employees in the Sales department, including their employee number, last name, first name, and department name.
7.	Listed all employees in the Sales and Development departments, including their employee number, last name, first name, and department name.
8.	In descending order, list the frequency count of employee last names, i.e., how many employees share each last name.

## SQL Alchemy
* Import the SQL database into Pandas using the following:
  from sqlalchemy import create_engine
* engine = create_engine('postgresql://localhost:5432/<your_db_name>')
connection = engine.connect()
* Create a histogram to visualize the most common salary ranges for employees.
* Create a bar chart of average salary by title. 

