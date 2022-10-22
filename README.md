# SQL
SQL code. HELP 



This is the SQL code for the client databases. You have noticed some duplicates in the customers table.
Below is the structure of the table with its two initial fields.
2 initial fields of the customer table



______________________________________________________
   
CREATE TABLE Customer( 
                            customerlD int PRIMARY KEY IDENTITY(1,1) 
NOT NULL, 
                            customerName varchar(50) NOT NULL, 

                             • • • 
)
_________________________________________________________

The query below is INCOMPLETE:


___________________________________________
;WITH CustomerCTE 
AS 
( 
            SELECT 
            customerName 
           ,ROW_NUMBER() OVER(PARTITION BY 
customername ORDER BY customername ) SeqNum 
            FROM customer

___________________________________________


Which of the following options will you use to complete the query?

a) WHERE SeqNum >2
b) WHERE SeqNum >1
c) WHERE SeqNum >0
d) WHERE SeqNum >=


Question 2:

True or false?
You can improve the performance of the SQL query below by adding the suggested index shown below when working with a large table.
SQL queries:
____________________
SELECT Name, Country 
FROM DBO.CUSTOMER 
WHERE Country=’USA' 
______________________

Suggested Index:
__________________________
CREATE NONCLUSTERED INDEX IX_Customer_Cty 
ON DBO.CUSTOMER (Country) 
INCLUDE (Name) 
_______________________


a) True
b) False

