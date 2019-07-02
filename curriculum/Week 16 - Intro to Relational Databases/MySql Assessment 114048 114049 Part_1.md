
# MySQL Assesment

## NCIT Units

## Instructions
- Save all of your instructions in a script file - you will submit this file on Gnomio and github.
- save it as `MySql Assessment 114048 & 114049 Part 1``

Download MySQL and install on Ubuntu:

```
sudo apt update
sudo apt upgrade
wget http://repo.mysql.com/mysql-apt-config_0.8.10-1_all.deb
sudo dpkg -i mysql-apt-config_0.8.10-1_all.deb
sudo apt update
sudo apt install mysql-server

```

 Run MySQL as root to complete the steps below: `mysql -u root `. You can run [mysql-workbench] (https://www.mysql.com/products/workbench/) to export your code in a script.

## Steps

2. Create a database called "Umuzi".

3. Create the following tables in Umuzi database
    - Customers
    - Employees
    - Orders
    - Payments
    - Products

4. Create a primary key for each table with auto-increment (make sure you correctly specify the data types, e.g. the ID field should be `int`).

5. Create foreign keys so that every ID in the order table references an existing ID in the tables referenced (e.g., ProductID, EmployeeID ...).

Create a query that will:

6. INSERT the following records to the tables described above:

### Customer Table

| CustomerID (int) | FirstName (varchar 50) | LastName (varchar 50) | Gender (varchar) | Address (varchar 200) | Phone (int 10) | Email (varchar 100) | City (varchar 20)| Country (varchar 50)|
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1	| John | Hibert | Male | 284 chaucer st| 084789657| john@gmail.com | Johannesburg | South Africa  |
| 2 | Thando | Sithole | Female | 240 Sect 1 | 0794445584 | thando@gmail.com | Cape Town | South Africa |
| 3 | Leon | Glen | Male | 81 Everton Rd,Gillits | 0820832830 | Leon@gmail.com | Durban | South Africa |
| 4 | Charl | Muller | Mal | 290A Dorset Ecke | +44856872553 | Charl.muller@yahoo.com | Berlin | Germany |
| 5 | Julia | Stein | Female | 2 Wernerring | +448672445058 | Js234@yahoo.com | Frankfurt | Germany |



### Employees Table

| EmployeeID (int) | FirstName (varchar 50) | LastName (varchar 50) |  Email (varchar 100) |  JobTitle (varchar 20) |
| --- | --- | --- | --- | --- |  
| 1 | Kani | Matthew | mat@gmail.com | Manager |
| 2 | Lesly | Cronje | LesC@gmail.com | Clerk |  
| 3 | Gideon | Maduku | m@gmail.com | Accountant |


### Orders Table

| OrderId (int) | ProductID (int) | PaymentID (int) | FulfilledByEmployeeID  (int) | DateRequired (datetime) | DateShipped (datetime) | Status (varchar 20) |  
| --- | --- | --- | --- |--- | --- |  --- |  
| 1  | 1  | 1  | 2  | 05-09-2018 | 02-09-2018 | Not shipped |
| 2  | 1  | 2  | 2  | 04-09-2018 | 03-09-2018 | Shipped |  
| 3  | 1  | 3  | 3  | 03-09-2018 | 02-09-2018 | Not shipped |  

### Payments Table

| CustomerId (int) | PaymentID (int) | PaymentDate (datetime) | Amount (decimal) |    
| --- | --- | --- | --- |   
| 1 | 1 | 01-09-2018 | R100.00 |  
| 2 | 2 | 01-09-2018 | R250.75 |  

### Products Table

| ProductId (int) | ProductName (varchar 100) | Description (varchar 300) | BuyPrice (decimal) |  
| --- | --- | --- | --- |  
| 1 | Harley Davidson Chopper | This replica features working kickstand, front suspension, gear-shift lever | R150.75 |
| 2 | Classic Car | Turnable front wheels, steering function | R550.75 |  
| 3 | Sports car | Turnable front wheels, steering function | R700.60 |

7. Document what information is stored in your database. Be sure to say what information is kept in what table, and which keys link the records between tables.
