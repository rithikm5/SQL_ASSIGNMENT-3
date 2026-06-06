# SQL_ASSIGNMENT-3
# Create a table shopping and insert values for different products.


CREATE TABLE Shopping (
    Product_ID INT PRIMARY KEY,
    Product_Name VARCHAR(50),
    Price DECIMAL(10,2),
    Quantity INT
);

INSERT INTO Shopping (Product_ID, Product_Name, Price, Quantity) VALUES
(101, 'Laptop', 55000, 10),
(102, 'Mobile', 25000, 15),
(103, 'Headphones', 2000, 30),
(104, 'Keyboard', 1500, 20),
(105, 'Mouse', 800, 25),
(106, 'Smart Watch', 5000, 12),
(107, 'Printer', 12000, 8),
(108, 'Monitor', 18000, 6);

# Print the products with highest and lowest price using aggregate functions

SELECT MAX(Price) AS Highest_Price, MIN(Price) AS Lowest_Price
FROM Shopping;
