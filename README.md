# Exploring Core SQL Syntax for Analyzing Celo Blockchain Transactions:

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Introduction:

The Celo blockchain is a decentralized platform that enables fast, secure, and low-cost payments and financial transactions using a native cryptocurrency called Celo. As with any blockchain, the Celo network generates a vast amount of data that can provide valuable insights into its operations, user behavior, and overall health. SQL is a powerful language that can be used to manage and analyze large datasets, making it an essential tool for those interested in exploring the Celo blockchain's transaction data. This tutorial will provide an overview of the fundamental SQL syntax necessary for analyzing Celo blockchain transactions. It will also cover basic SQL queries. The insights gained from SQL analysis can be used to inform Celo blockchain development, improve the user experience, and drive adoption.
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

*  [Let's dive into a practical example to demonstrate how to extract information from a Celo transaction using SQL.](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#lets-dive-into-a-practical-example-to-demonstrate-how-to-extract-information-from-a-celo-transaction-using-sql)

     - [Creating a Database](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#creating-a-database)
       - [Importing the Flat Files ( CSV ) into SQL Server](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#importing-the-flat-files--csv--into-sql-server)
       - [Calling the table from the Database ](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#calling-the-table-from-the-database)
       - [Find transaction details for a specific transaction ID](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#find-transaction-details-for-a-specific-transaction-id)
       - [Calculate the total amount transferred in the transaction](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#calculate-the-total-amount-transferred-in-the-transaction)
       - [Determine the gas fee paid for the transaction](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#determine-the-gas-fee-paid-for-the-transaction)
       - [Time functions used in Querying Celo Blockchain](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#time-functions-used-in-querying-celo-blockchain)

* [Conclusion](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#conclusion)
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Objectives:

The objective of this tutorial is to provide a comprehensive understanding of SQL syntax, which is necessary for analyzing Celo blockchain transactions. The tutorial aims to introduce the basics of SQL queries Through this, programmers will gain the necessary skills to query and analyze Celo blockchain data effectively. The ultimate objective is to empower programmers to use SQL as a tool for gaining valuable insights into the Celo blockchain's operations, user behavior, and overall health, leading to improvements in development, user experience, and adoption of the network.


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

1.Querying blockchain data: SQL provides a standardized way of querying data stored in the Celo blockchain, allowing developers and analysts to retrieve specific information quickly and efficiently. This can help identify patterns and insights that can be used to improve the network's performance.

2.Faster analysis: SQL queries can be optimized for performance by allowing faster analysis of large datasets. This can be particularly useful for analyzing transaction data and identifying performance bottlenecks or potential security issues.

3.Integration with other tools: SQL is widely used in the tech industry and many tools & platforms are built around it. Using SQL in Celo blockchain makes it easier to integrate it with other systems and tools which allows developers to leverage existing infrastructure and tools to build more robust applications.

4.Standardization: Using SQL in Celo blockchain provides a standardized way of interacting with the blockchain data, making it easier for developers and analysts to collaborate and share their work.

5.Transferable skills: Learning SQL is a valuable skill that can be applied to other relational databases and technologies. This means that developers and analysts who learn SQL in the context of Celo blockchain can apply their skills to other projects and industries, making it a valuable skill to have in today's job market.

Overall, using SQL in Celo blockchain can help developers and analysts to efficiently, effectively manage and analyze the network's data, leading to better performance and a more robust blockchain ecosystem.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Let's dive into a practical example to demonstrate how to extract information from a Celo transaction using SQL:
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





* ## Let's say we have a Celo_transactions table with the following columns: ```transaction_id```, ```sender_address```, ```receiver_address```, ```amount```, ```gas_fee```, and ```transaction_date```. The goal is to analyze a specific transaction and extract relevant information.

*  ## Find transaction details for a specific transaction ID:



``` 
-- To extract details for a specific transaction, you can use the following SQL query:

SELECT *  -- This statement selects all columns from the table.

FROM Celo_transactions  -- Specifies the table from which to retrieve the data 

WHERE transaction_id = 'your_transaction_id'; -- This condition filters the rows based on the transaction_id column.

```

* ## Calculate the total amount transferred in the transaction:

```
-- To calculate the total amount transferred in a transaction, you can use the following query:

SELECT SUM(amount) AS total_amount -- This statement calculates the sum of the amount column for the selected transaction and assigns it an alias of total_amount. 

FROM Celo_transactions              -- Specifies the table from which to retrieve the data 

WHERE transaction_id = 'your_transaction_id';   -- This condition filters the rows based on the transaction_id column.


```

* ## Determine the ```gas_fee``` paid for the transaction:

```
-- To find the gas_fee paid for a specific transaction, you can use the following query:

SELECT gas_fee   -- This statement specifies the column gas_fee that you want to retrieve from the table. It indicates that you are interested in obtaining the gas fee associated with the transaction.

FROM Celo_transactions  --   Specifies the table from which to retrieve the data 

WHERE transaction_id = 'your_transaction_id'; -- This condition filters the rows based on the transaction_id column.


```

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Time functions used in Querying Celo Blockchain:

* Analyze transactions within a specific date range:




```
To analyze transactions within a specific date range, you can use the following query:

SELECT *   -- This statement selects all columns from the table.

FROM Celo_transactions -- Specifies the table from which to retrieve the data 

WHERE transaction_date >= 'start_date' AND transaction_date <= 'end_date';  -- This condition filters the rows based on the transaction_date column. It selects only the rows where the transaction date is greater than or equal to the specified start date and less than or equal to the specified end date.


```



These examples demonstrate how you can extract specific information from Celo transactions using SQL queries. By modifying the queries based on your analysis requirements, you can gain insights into transaction data, such as specific transaction details, total amounts transferred, gas fees, and analyzing transactions within a specific date range.


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## CONCLUSION:

SQL is a crucial tool for analyzing Celo blockchain transactions. By understanding SQL syntax and employing querying techniques, developers can effectively extract information from Celo transactions, gaining valuable insights for development, user experience, and adoption decisions.



