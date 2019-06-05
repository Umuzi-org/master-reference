# MySql Assessment
# NCIT units 114048 & 114049

## Instructions
Save all of your instructions in a script file - you will submit this file on Gnomio and github.

Download MySQL and install on Ubuntu; also install the MySQLdb library in python (using conda or pip install).
The MySQLdb package will allow you to use python to interface with your MySQL database.


## Questions

1. Open a mySQL connection in python.
2. Create a database called "Umuzi".

3. Create the following tables
    - Customers
    - Employees
    - Orders
    - Payments
    - Products

4. Create a Primary key for each table with auto-increment (make sure you correctly specify the data types, e.g. the ID field should be `int`).
5. Create a Foreign key for the tables.

Create a query that will:

6. INSERT the following records to the tables described above.

### Customer Table

| CustomerID | FirstName | LastName | Gender | Address | Phone | Email | City | Country |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1	| John | Hibert | Male | 284 | chaucer st	| 084789657 (int 10) | john@gmail.com (varchar 100) | Johannesburg | South Africa |
| 2 | Thando | Sithole | Female | 240 Sect 1 | 0794445584 | thando@gmail.com (varchar 100) | Cape Town | South Africa |
| 3 | Leon | Glen | Male | 81 Everton Rd,Gillits | 0820832830 | Leon@gmail.com (varchar 100) | Durban | South Africa |
| 4 | Charl | Muller | Mal | 290A Dorset Ecke | +44856872553 | Charl.muller@yahoo.com (varchar 100) | Berlin | Germany |
| 5 | Julia | Stein | Female | 2 Wernerring | +448672445058 | Js234@yahoo.com (varchar 100) | Frankfurt | Germany |



### Employees Table

| EmployeeID
 | FirstName | Last Name | Email |
 Job Title |  
| --- | --- | --- | --- | --- |  
| 1 (int) | Kani (varchar 50) | Matthew (varchar 50) | mat@gmail.com (varchar 100) | Manager |  

| 2 (int) | Lesly (varchar 50) |
Cronje (varchar 50) | LesC@gmail.com (varchar 100) | Clerk |  

| 3 (int) |
Gideon (varchar 50) | Maduku (varchar 50) | m@gmail.com (varchar 100) | Accountant |
  

### Orders Table

| OrderId |
 Order | Date
Required | Date
Shipped |
Status |  
| --- | --- | --- | --- |--- |  

| 1 (int) |
 01-09-2018 (datetime) | 05-09-2018 | 02-09-2018 | Not shipped |  
| 2 (int) |
 01-09-2018 (datetime) | 04-09-2018 | 0
3-09-2018 | Shipped
 |  
| 3 (int) | 01-09-2018 (datetime) |
 03-09-2018
 | 02-09-2018 | Not shipped
 |  

### Payments Table

| CustomerId | PaymentDate |
 Amount |    
| --- | --- | --- |  
| 1 (int) | 01-09-2018 (datetime) | R100.00 (decimal) |  
| 2 (int) | 01-09-2018 (datetime) | R250.75 (decimal)
 |  

### Products Table

| ProductId | ProductName |
 Description | BuyPrice |  
| --- | --- | --- | --- |  
| 1 (int) |
 Harley Davidson Chopper | This replica features working kickstand, front suspension, gear-shift lever | R150.75 (decimal) |  

| 2 (int) |
 Classic Car | Turnable front wheels, steering function | R550.75 (decimal) |  
| 3 (int) | Sports car | Turnable front wheels, steering function |
 R700.60
 (decimal) |     


7. SELECT ALL records from table Customers.

8. SELECT records only from the name column in the Customers table.

9. Show the name of the Customer whose CustomerID is 1.

10. UPDATE the record for CustomerID =1  on the Customer table so that the name is "Lerato Mabitso".

11. DELETE the record from the Customers table for customer 2 (CustomerID = 2).

12. Select all unique values from the table Products.

13. Return the MAXIMUM payment made on the PAYMENTS table.

14. Create a query that selects all customers from the "Customers" table, sorted by the "Country" column.

15. Create a query that selects all Products with a price BETWEEN R100 and R600.

16. Create a query that selects all fields from "Customers" where country is "Germany" AND city is "Berlin".

17. Create a query that selects all fields from "Customers" where city is "Cape Town" OR "Durban".

18. Select all records from Products where the Price is GREATER than R500.

19. Return the sum of the Amounts on the Payments table.

20. Count the number of shipped orders in the Orders table.

21. Return the average price of all Products, in Rands and in Dollars (assume the exchange rate is R12 to the Dollar).

22. Using INNER JOIN create a query that selects all Payments with Customer information.

23. Document what information is stored in your database. Be sure to say what information is kept in what table, and which keys link the records between tables.
