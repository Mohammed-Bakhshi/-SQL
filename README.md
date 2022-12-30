W3school SQL https://www.w3schools.com/sql/sql_groupby.asp
using the w3scool SQL environment I Joined 3 separate table together
Customer Name	Order Date	Shipper Name	ProductName.

first code 

SELECT Customers.CustomerName, Orders.OrderDate,Shippers.ShipperName,Products.ProductName
FROM Customers,Shippers,Products
CROSS JOIN Orders
WHERE OrderDate= '1996-07-04' AND  ShipperName ='United Package' ;

        



Secondly i use the same tables but this typr i only got the data from 1996 and counting how maqnny product was brought of each item in that year 

this is my code 

SELECT COUNT(Orders.OrderDate),Products.ProductName
FROM Products
CROSS JOIN Orders
WHERE "1996"
GROUP BY OrderDate;

