# MySql Assessment
# NCIT units 114048 & 114049

## Instructions
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

| CustomerID  |
|-------------|------------|----------|---------|-------------------------|----------------|-------------------------|---------------|--------------|


|

| 5


### Employees Table

| EmployeeID
|-------------|--------------------|----------------------|--------------------------------|-------------|  
| 1 (int)     | Kani (varchar 50)  | Matthew (varchar 50) | mat@gmail.com (varchar 100)    | Manager     |  



### Orders Table

| OrderId     |
|-------------|------------------------|-----------------|----------------|----------------|  
| 1 (int)     |
| 2 (int)     |
| 3 (int)     | 01-09-2018 (datetime)  |

### Payments Table

| CustomerId      | PaymentDate           |
|-----------------|-----------------------|-------------------|  
| 1 (int)         |
| 2 (int)         | 01-09-2018 (datetime) |

### Products Table

| ProductId
|------------|-------------------------|-----------------------------------------------------------------------------|--------------------|  
| 1 (int)    |

| 3 (int)


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