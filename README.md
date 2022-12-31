# SQl
## Joing 3 tables in SQL 

using the w3school envioment https://www.w3schools.com/sql/  

 First half i joined 3 tables together from products,orders and customers then i made it only show the shipper name as United Package and the order date 1996-7-4.    

Secondly I Created a second SQL query that uses the same database, however the data returned had 2 columns, ProductName from the products database and a second column with the total sales in 2017 for each product.  
### First Part Of SQL Code 

 SELECT Customers.CustomerName, Orders.OrderDate,Shippers.ShipperName,Products.ProductName FROM Customers,Shippers,Products CROSS JOIN Orders WHERE OrderDate= '1996-07-04' AND ShipperName ='United Package' ; 

### Second Part Of SQL code 

SELECT COUNT(Orders.OrderDate),Products.ProductName
FROM Products  
CROSS JOIN Orders
WHERE "1996"
GROUP BY OrderDate;

