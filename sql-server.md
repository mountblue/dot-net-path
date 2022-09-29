# SQL Server

## Setup

For this section, you will need to install SQL Server. Both the regular or express version is acceptable.

Also, install SQL Server Management Studio, which comes up as part of the installation of SQL Server.

The following video explains the whole process.
[https://www.youtube.com/watch?v=QsXWszvjMBM](https://www.youtube.com/watch?v=QsXWszvjMBM)

## SQL Basics

The following tutorial takes you through the basics of SQL, specifically with SQLServer.

[https://www.youtube.com/watch?v=JTDK6r1GuUU](https://www.youtube.com/watch?v=JTDK6r1GuUU)

## ADO.NET

Connect to SQLServer from C# with ADO.NET.

The following tutorial takes you through the basics of ADO.NET.

[ADO.NET playlist](https://www.youtube.com/watch?v=RriFg1AFoT0&list=PLWPirh4EWFpFMkh4NFDzascBGWJ-E3zO8)

### Data Project - ADO.NET Version

*NOTE* The database for this project is SQLServer

#### Target
In this assignment you will solve the sample problems as the first data assignment, But, in this case, your raw data will come from the database and not from a CSV file.

Your C# program should take in one command-line argument. It should either be the string "load" or "analyze". If any other argument is given it should print an error message and exit.

#### Loader

If the argument is "load" then you should run the loader.

The loader should ...
1. Create the database if it does not exist.
2. Create the table if it does not exist.
2. Read the CSV file and add the data from the CSV file to the database.

#### Analyzer

If the argument is "analyze" then you should run the analyzer.

The analyzer should ...
1. Query the database for the 4 problems.
2. Print the results in table format as in the previous assignment.
