# Exploring Core SQL Syntax for Analyzing Celo Blockchain Transactions:

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Introduction:

Celo blockchain enables fast, secure, and low-cost payments using Celo cryptocurrency. SQL is essential for analyzing its transaction data. This tutorial covers SQL basics and querying to gain insights for development, user experience, and adoption.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Table of Contents:

* [Exploring the Core SQL Syntax for Analyzing Celo Blockchain Transactions](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#exploring-the-core-sql-syntax-for-analyzing-celo-blockchain-transactions)

  - [Introduction](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#introduction)
  - [Table of Contents](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#table-content)
  - [Objectives](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#objectives)
  - [Pre-requisites](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#prerequisites)
  - [Requirements](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#requirements)
  - [Sample Data Source](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#sample-data-source)
  
   - [Explaining the use of SQL in Web3](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#explaining-the-use-of-sql-in-web3)
      - [Benefits of using SQL in CELO Blockchain](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#benefit-of-using-sql-in-celo-blockchain)

* [Tutorial](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#tutorial)

     - [Creating a Database](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#creating-a-database)
       - [Importing the Flat Files ( CSV ) into SQL Server](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#importing-the-flat-files--csv--into-sql-server)
       - [Calling the table from the Database ](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#calling-the-table-from-the-database)
       - [How to use all Aggregate Functions](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#how-to-use-all-aggregate-functions-and-date-functions-will-be-covered-in-the-tutorial)
       - [How to use Time Functions](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#time-functions-used-in-querying-celo-blockchain)

* [Conclusion](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#conclusion)
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Objectives:

This tutorial teaches programmers SQL syntax for analyzing Celo blockchain transactions. By mastering SQL queries, programmers can effectively query and analyze Celo blockchain data, gaining valuable skills for data analysis.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Pre-requisites:

* How to analyze CELO data with SQL?
* Recognizing the fundamental operations utilized to create the CELO Data dashboard.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Requirements: 

* SQL EDITOR: SQL editors are essential tools for anyone working with relational databases and SQL queries. They provide a user-friendly interface for writing and executing SQL code, making it easier to manage and analyze data stored in a database.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Sample Data Source:

*  This is the link to the [Data Source](https://celoscan.io/exportData?type=internaltxns&a=0x3d90ec3c3272b66ee2b0170c249bfaa3ee59cc94) 

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

 ## Explaining the use of SQL in Web3:
 
 * SQL is a versatile tool that can be used for a variety of Web3 applications including blockchain analysis, decentralized storage, and dApp development. Its ability to query and analyze structured data makes it a powerful tool for managing and analyzing data in decentralized systems.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Benefits of using SQL in CELO Blockchain:

There are several benefits to using SQL in Celo blockchain which are as follows:

1.**Querying blockchain data**: SQL provides a standardized way of querying data stored in the Celo blockchain, allowing developers and analysts to retrieve specific information quickly and efficiently. This can help identify patterns and insights that can be used to improve the network's performance.

2.**Faster analysis**: SQL queries can be optimized for performance by allowing faster analysis of large datasets. This can be particularly useful for analyzing transaction data and identifying performance bottlenecks or potential security issues.

3.**Integration with other tools**: SQL is widely used in the tech industry and many tools & platforms are built around it. Using SQL in Celo blockchain makes it easier to integrate it with other systems and tools which allows developers to leverage existing infrastructure and tools to build more robust applications.

4.**Standardization**: Using SQL in Celo blockchain provides a standardized way of interacting with the blockchain data, making it easier for developers and analysts to collaborate and share their work.

5.**Transferable skills**: Learning SQL is a valuable skill that can be applied to other relational databases and technologies. This means that developers and analysts who learn SQL in the context of Celo blockchain can apply their skills to other projects and industries, making it a valuable skill to have in today's job market.

Overall, using SQL in Celo blockchain can help developers and analysts to efficiently, effectively manage and analyze the network's data, leading to better performance and a more robust blockchain ecosystem.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Tutorial:
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Creating a Database:

Once you have executed this SQL command, a new database with the name celo_blockchain will be created in your SQL server. Note that you will need appropriate permissions and access to the SQL server in order to create a new database.

```
CREATE DATABASE celo_blockchain;

```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Importing the Flat Files ( CSV ) into SQL Server:

1.```file_path``` is the path to the CSV file that you want to import.

2.```Celo_transactions``` is the name of the table where you want to import the data.

3.```FIELDS TERMINATED BY ','``` specifies that the fields in the CSV file are separated by commas.

4.```ENCLOSED BY '"'``` specifies that fields are enclosed by double quotes.

5.```LINES TERMINATED BY '\n'``` specifies that each row is terminated by a new line character.

6.```IGNORE 1 ROWS``` tells the SQL engine to ignore the first row in the CSV file, which is usually a header row.

Here is an example of how you might use this syntax to import data from a CSV file named my_data.csv into a table named my_table:

```
-- This code disables foreign key checks, loads data from a CSV file into the celo_name table, and re-enables foreign key checks.

SET FOREIGN_KEY_CHECKS = 0;    -- This line disables foreign key checks to speed up the loading process and avoid foreign key constraints errors.

LOAD DATA INFILE '/absolute/path/to/my_celo.csv'      -- This loads the data from the specified CSV file into the celo_name table.
INTO TABLE celo_name
CHARACTER SET utf8        -- This specifies the character set of the CSV file to be UTF-8.
FIELDS TERMINATED BY ','   -- This specifies that the fields in the CSV file are separated by commas.
ENCLOSED BY '"'     -- This specifies that fields that contain commas are enclosed in double quotes.
LINES TERMINATED BY '\n'   -- This specifies that each line in the CSV file ends with a newline character.
IGNORE 1 ROWS        -- This specifies that the first row of the CSV file should be ignored as it usually contains the header.

ERRORS;        -- This line specifies that any errors encountered during the load process should be displayed as warnings and the loading process should continue.

SET FOREIGN_KEY_CHECKS = 1;        -- This line re-enables foreign key checks after the loading process is complete.


```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Calling the Table from the Database:

```SELECT * FROM Celo_transactions;```

In this syntax,```Celo_transactions``` is the name of the table you want to select data from. The ```*``` symbol specifies that you want to select all columns from the table
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## How to use all Aggregate Functions:

* The aggregate functions will be our first focus.

Aggregate functions in SQL are functions that perform a calculation on a set of values and return a single value. 

* ```COUNT()```: returns the number of rows that match a specified condition.
* ```SUM()```: returns the sum of all values in a specified column.
* ```AVG()```: returns the average of all values in a specified column.
* ```MIN()```: returns the smallest value in a specified column.
* ```MAX()```: returns the largest value in a specified column.

* ## To find the total transactions:

``` 
-- This query calculates the total number of transactions stored in the Celo_transactions table.


SELECT SUM(txns) AS "Total_Transactions" -- This calculates the sum of the txns column of all transactions and gives the result a column alias "Total_Transactions".

FROM Celo_transactions; -- This specifies the Celo_transactions table as the source of data for the query.

```

* ## To find the average block time:

```
-- This query calculates the average block time of all transactions stored in the Celo_transactions table.

SELECT AVG(age) AS "Avg_block_time" -- This calculates the average block time of all transactions and gives the result a column alias "Avg_block_time".

FROM Celo_transactions; -- This specifies the Celo_transactions table as the source of data for the query.

```

* ## To find the average gas fee:

```
-- This query calculates the average gas fee of all transactions stored in the Celo_transactions table.

SELECT AVG(gas_fee) AS "Avg_gas_fee" -- This calculates the average gas fee of all transactions and gives the result a column alias "Avg_gas_fee".

FROM Celo_transactions; -- This specifies the Celo_transactions table as the source of data for the query.

```

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Time functions used in Querying Celo Blockchain:

* Time functions in SQL are used to work with temporal data such as dates and times. These functions provide a way to extract or manipulate specific parts of a date or time value, perform calculations on dates and times, and format date and time values for display.

```NOW()```: returns the current date and time.
```DATE()```: extracts the date part of a date/time value.
```TIME()```: extracts the time part of a date/time value.
```YEAR(),``` MONTH(), DAY(): extract the year, month, or day from a date value.
```HOUR(),``` MINUTE(), SECOND(): extract the hour, minute, or second from a time value.
```DATEDIFF()```: calculates the difference between two dates or times.

* ## To find the days of  Carbon Nagative Celo blockchain:

* Assuming you have a table named Celo_transactions with columns ***id***, ***date***, and ***carbon_negative***, where date stores the transaction date and carbon_negative stores a boolean value indicating whether the transaction is carbon negative, you can use the following SQL query to calculate the number of days between the current date and the transaction date, and include the carbon_negative column:

```
-- This query selects the id, the number of days since the date of the transaction, and the carbon negative value 
-- from the Celo_transactions table.

SELECT id, 
       DATEDIFF(NOW(), date) AS Days_carbon_negative, -- This calculates the number of days between the transaction date and today's date.
       
       carbon_negative -- This selects the carbon negative value from the Celo_transactions table.
FROM Celo_transactions;

```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## CONCLUSION:

Hence, SQL is a powerful tool for analyzing Celo blockchain transactions. With the vast amount of transaction data generated on the blockchain, SQL provides a flexible and efficient way to extract and manipulate the data. By understanding the core syntax of SQL and its functions, users can query the blockchain database to extract meaningful insights such as transaction volume, block time, gas prices, and carbon footprint. These insights can help to inform decisions related to blockchain development, adoption and sustainability. As the Celo blockchain continues to grow and evolve, the ability to analyze and make sense of the transaction data becomes increasingly important. By mastering the core SQL syntax for analyzing Celo blockchain transactions, users can stay ahead of the curve and unlock the full potential of the blockchain.



