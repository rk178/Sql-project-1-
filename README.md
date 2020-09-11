# Sql-project-1-
Data Analysis of AdventureWorks 2014 Datawarehousing database 

Dataset :- AdventureWorks 2014 Datawarehousing Database (ms sql)
Url:- https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-serverver15&
tabs=ssms
Database file Name- AdventureworksDW2014.bak (ms sql file)



Asking some questions to the database to find relative information:-
Q1.Q1. Find First name and DOB of from the table Dimcustomer present in the database?
Ans. Queries used:-
First select Dimcustomer table from database,
-- SELECT * FROM DimCustomer;(query used)
Then find firstname and DOB from the Dimcustomer table,
-- SELECT FirstName, Birthdate from Dimcustomer;(query used)


Q2. Select from tables Dimcustomer column name YearlyIncome put the yearly income in descending
order?
Ans. With below used query put the yearlyncome values in descending order:-
Query used:- SELECT * FROM DimCustomer ORDER BY YearlyIncome DESC;
Desc;(means descending)



Q3. Select Yearly Income greater than 60000.00 ( > 60000.00) from table Dimcustomer ?
Ans.From the below query we can show yearly income greater than > 60000.00 ( > 60000.00 used to display
value above mention numbers)
Query used:- Select * from DimCustomer where YearlyIncome > 60000.00;





Q4. Create a table in the database name yearlyprofit with varchar and floating numbers ?
Ans. create a table with below query:
Note: Create table-for creating the table, varchar and float are data types: -
CREATE TABLE Yearlyprofit (
COMPANY_NAME VARCHAR,
CLIENT_NAME VARCHAR,
LOSS FLOAT,
PROFIT FLOAT,
);




Q5. Find the martial status in Dimcustomer table who are single (S)?
Ans:- First select dimcustomer with below query used
Query used:- SELECT * FROM DimCustomer;
Then select the Martialstatus column from the Dimcustomer table by below used
query to find single person denoted by S(single) and M(married)present in the
table bur we have to find the single one’s in the table.
SELECT * FROM DimCustomer WHERE MaritalStatus = 'S';(s for single)
