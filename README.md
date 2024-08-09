1...Data cleaning
2...Remove duplicates
3...standardize the data
4...null values or blanks values
5...remove any columns


... Data cleaning


Select *
from retail_sales_dataset;




CREATE TABLE retailworld 
like retail_sales_dataset;

select * FROM retailworld;

Insert retailworld
SELECT * from retail_sales_dataset;

select * FROM retailworld;


SELECT *,
ROW_NUMBER() OVER(PARTITION BY TransactionID,CustomerID,Gender,Age.ProductCategory,Quantity,Priceperunit, Total, `Date`) AS row_num
FROM retailworld;
