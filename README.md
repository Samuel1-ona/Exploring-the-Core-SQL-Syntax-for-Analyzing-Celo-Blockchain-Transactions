# Exploring the Core SQL Syntax for Analyzing Celo Blockchain Transactions

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
# INTRODUCTION

The Celo blockchain is a decentralized platform that enables fast, secure, and low-cost payments and financial transactions using a native cryptocurrency called CELO. As with any blockchain, the Celo network generates a vast amount of data that can provide valuable insights into its operations, user behavior, and overall health. SQL is a powerful language that can be used to manage and analyze large datasets, making it an essential tool for those interested in exploring the Celo blockchain's transaction data. This topic, "Exploring the Core SQL Syntax for Analyzing Celo Blockchain Transactions," will provide an overview of the fundamental SQL syntax necessary for analyzing Celo blockchain transactions. It will cover basic SQL queries such as `SELECT`, `WHERE`, and `GROUP BY`, as well as more advanced functions like `JOIN` and subqueries. The insights gained from SQL analysis can be used to inform Celo blockchain development, improve user experience, and drive adoption.


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
# TABLE CONTENT
* [Exploring the Core SQL Syntax for Analyzing Celo Blockchain Transactions](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#exploring-the-core-sql-syntax-for-analyzing-celo-blockchain-transactions)

  - [INTRODUCTION](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#introduction)
  - [TABLE CONTENT](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#table-content)
  - [OBJECTIVES](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#objectives)
  - [PREREQUISITES](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#prerequisites)
  - [REQUIREMENTS ](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#requirements)
  - [SAMPLE DATA SOURCE](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#sample-data-source)
  
   - [EXPLAINING THE USE OF SQL IN WEB3](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#explaining-the-use-of-sql-in-web3)
      - [BENEFIT OF USING SQL IN CELO BLOCKCHAIN ](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#benefit-of-using-sql-in-celo-blockchain)

* [TUTORIAL](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#tutorial)

     - [CREATING A DATABASE](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#creating-a-database)
       - [IMPORTING THE FLAT FILES ( CSV ) INTO SQL SERVER ](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#importing-the-flat-files--csv--into-sql-server)
       - [CALLING THE TABLE FROM THE DATABASE ](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#calling-the-table-from-the-database)
       - [HOW TO USE ALL AGGREGATE FUNCTIONS](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#how-to-use-all-aggregate-functions-and-date-functions-will-be-covered-in-the-tutorial)
       - [HOW TO USE TIME FUNCTIONS](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#time-functions-used-in-querying-celo-blockchain)

* [CONCLUSION](https://github.com/Samuel1-ona/Exploring-the-Core-SQL-Syntax-for-Analyzing-Celo-Blockchain-Transactions/blob/main/README.md#conclusion)
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
# OBJECTIVES

The objective of "Exploring the Core SQL Syntax for Analyzing Celo Blockchain Transactions" is to provide a comprehensive understanding of SQL syntax necessary for analyzing Celo blockchain transactions. The topic aims to introduce the basics of SQL queries such as `SELECT`, `WHERE`, and `GROUP BY`, and to explore more advanced functions such as `JOIN` and subqueries. Through this exploration of SQL syntax, readers will gain the necessary skills to query and analyze Celo blockchain data effectively. The ultimate objective is to empower readers to use SQL as a tool for gaining valuable insights into the Celo blockchain's operations, user behavior, and overall health, leading to improvements in development, user experience, and adoption of the network.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------


# PREREQUISITES

Before diving into the core SQL syntax for analyzing Celo blockchain transactions, it is essential to have a fundamental understanding of SQL concepts and principles. Some basic SQL concepts include:

- Database design and management
- Tables, columns, and data types
- Data manipulation using CRUD operations (CREATE, READ, UPDATE, DELETE)
- Basic SQL queries such as `SELECT`, `FROM`, `WHERE`, and `GROUP BY`

Familiarity with these concepts will make it easier to follow along with the tutorial and understand the SQL syntax used to analyze Celo blockchain transactions. Additionally, it is helpful to have a basic understanding of blockchain technology and the Celo blockchain specifically.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# GOALS

* Understanding how to analyze CELO data with SQL.
* Recognizing the fundamental operations utilized to create the CELO Data dashboard.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# REQUIREMENTS

### To follow this tutorial, you should have a basic understanding of the Celo blockchain and its transactions. You should also have access to a SQL server, such as MySQL, PostgreSQL, or SQL Server, and have a basic understanding of SQL syntax.

The following software and tools will be used in this tutorial:

 - A SQL server, such as MySQL, PostgreSQL, or SQL Server
 - A command-line interface or GUI for interacting with the SQL server
 - A text editor or SQL client for writing and executing SQL queries
 - Basic knowledge of SQL syntax

Optional:

- Basic knowledge of command line interface
- Basic knowledge of Python/ any programming language

### It is not necessary to have prior experience with analyzing blockchain data or SQL, as this tutorial will provide an introduction to both. However, it is recommended to have some prior experience with SQL syntax and databases.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# SAMPLE DATA SOURCE

*  This is the link to the [Data Source](https://celoscan.io/exportData?type=internaltxns&a=0x3d90ec3c3272b66ee2b0170c249bfaa3ee59cc94) 

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

 ## EXPLAINING THE USE OF SQL IN WEB3
 
 * SQL is a versatile tool that can be used in a variety of Web3 applications, including blockchain analysis, decentralized storage, and dApp development. Its ability to query and analyze structured data makes it a powerful tool for managing and analyzing data in decentralized systems.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## BENEFIT OF USING SQL IN CELO BLOCKCHAIN 

There are several benefits to using SQL in Celo blockchain, including:

1.Querying blockchain data: SQL provides a standardized way of querying data stored in the Celo blockchain, allowing developers and analysts to retrieve specific information quickly and efficiently. This can help identify patterns and insights that can be used to improve the network's performance.

2.Faster analysis: SQL queries can be optimized for performance, allowing for faster analysis of large datasets. This can be particularly useful for analyzing transaction data and identifying performance bottlenecks or potential security issues.

3.Integration with other tools: SQL is widely used in the tech industry, and many tools and platforms are built around it. Using SQL in Celo blockchain makes it easier to integrate with other systems and tools, allowing developers to leverage existing infrastructure and tools to build more robust applications.

4.Standardization: SQL is a standardized language that is widely used across the tech industry. Using SQL in Celo blockchain provides a standardized way of interacting with the blockchain data, making it easier for developers and analysts to collaborate and share their work.

5.Transferable skills: Learning SQL is a valuable skill that can be applied to other relational databases and technologies. This means that developers and analysts who learn SQL in the context of Celo blockchain can apply their skills to other projects and industries, making it a valuable skill to have in today's job market.

Overall, using SQL in Celo blockchain can help developers and analysts more efficiently and effectively manage and analyze the network's data, leading to better performance and a more robust blockchain ecosystem.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------


# TUTORIAL 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## CREATING A DATABASE 

Once you have executed this SQL command, a new database with the name celo_blockchain will be created in your SQL server. Note that you will need appropriate permissions and access to the SQL server in order to create a new database.

```
CREATE DATABASE celo_blockchain;

```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## IMPORTING THE FLAT FILES ( CSV ) INTO SQL SERVER 

1.```file_path``` is the path to the CSV file that you want to import.

2.```Celo_transactions``` is the name of the table where you want to import the data.

3.```FIELDS TERMINATED BY ','``` specifies that the fields in the CSV file are separated by commas.

4.```ENCLOSED BY '"'``` specifies that fields are enclosed by double quotes.

5.```LINES TERMINATED BY '\n'``` specifies that each row is terminated by a new line character.

6.```IGNORE 1 ROWS``` tells the SQL engine to ignore the first row in the CSV file, which is usually a header row.

Here is an example of how you might use this syntax to import data from a CSV file named my_data.csv into a table named my_table:

```
LOAD DATA INFILE '/path/to/my_celo.csv'
INTO TABLE celo_name
FIELDS TERMINATED BY ','
ENCLOSED BY '"'
LINES TERMINATED BY '\n'
IGNORE 1 ROWS;

```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## CALLING THE TABLE FROM THE DATABASE 

```SELECT * FROM Celo_transactions;```

In this syntax,```Celo_transactions``` is the name of the table you want to select data from. The ```*``` symbol specifies that you want to select all columns from the table
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## HOW TO USE ALL AGGREGATE FUNCTIONS

* The aggregate functions will be our first focus.

Aggregate functions in SQL are functions that perform a calculation on a set of values and return a single value. 


* ```COUNT()```: returns the number of rows that match a specified condition.
* ```SUM()```: returns the sum of all values in a specified column.
* ```AVG()```: returns the average of all values in a specified column.
* ```MIN()```: returns the smallest value in a specified column.
* ```MAX()```: returns the largest value in a specified column.

* ## To find the total transactions

``` 
SELECT SUM(txns)
AS "Total_Transactions"
FROM Celo_transactions;
```

* ## To find the average block time 

```
SELECT AVG(age)
AS " Avg_block_time"
FROM Celo_transactions;

```

* ## To find the average gas fee 

```
SELECT AVG(gas_fee)
AS " Avg_gas_fee"
FROM Celo_transactions;

```

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Time functions used in Querying Celo Blockchain

* Time functions in SQL are used to work with temporal data, such as dates and times. These functions provide a way to extract or manipulate specific parts of a date or time value, perform calculations on dates and times, and format date and time values for display.

```NOW()```: returns the current date and time.
```DATE()```: extracts the date part of a date/time value.
```TIME()```: extracts the time part of a date/time value.
```YEAR(),``` MONTH(), DAY(): extract the year, month, or day from a date value.
```HOUR(),``` MINUTE(), SECOND(): extract the hour, minute, or second from a time value.
```DATEDIFF()```: calculates the difference between two dates or times.

* ## To find the days of  Carbon Nagative Celo blockchain .

* Assuming you have a table named Celo_transactions with columns ***id***, ***date***, and ***carbon_negative***, where date stores the transaction date and carbon_negative stores a boolean value indicating whether the transaction is carbon negative, you can use the following SQL query to calculate the number of days between the current date and the transaction date, and include the carbon_negative column:

```
SELECT id, DATEDIFF(NOW(), date)
AS Days_carbon_negative,
carbon_negative
FROM Celo_transactions;
```
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## CONCLUSION

In conclusion, SQL is a powerful tool for analyzing Celo blockchain transactions. With the vast amount of transaction data generated on the blockchain, SQL provides a flexible and efficient way to extract and manipulate the data. By understanding the core syntax of SQL and its functions, users can query the blockchain database to extract meaningful insights, such as transaction volume, block time, gas prices, and carbon footprint. These insights can help to inform decisions related to blockchain development, adoption, and sustainability. As the Celo blockchain continues to grow and evolve, the ability to analyze and make sense of the transaction data becomes increasingly important. By mastering the core SQL syntax for analyzing Celo blockchain transactions, users can stay ahead of the curve and unlock the full potential of the blockchain.



