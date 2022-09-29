# C# and .NET Development

## Setup

### Install Visual Studio
You will need a working Visual Studio 2019 environment to develop .NET Apps. So go ahead and set that up.

#### [OPTIONAL] Visual Studio setup instruction.

The setup is quite straight forward. In case you need more help, the following video shows you how to setup Visual Studio 2019.

[https://www.youtube.com/watch?v=G1-Zfr9-3zs](https://www.youtube.com/watch?v=G1-Zfr9-3zs)

## Basics of C# language

The following video is an informal intro to the C# language.

#### IMPORTANT
- Code along with the tutorial. Do not just watch the tutorial, **WRITE CODE** along with the tutorial. The only way to learn coding is writing code.

#### Alternate material
The following video is just a suggestion from me. There are A LOT of great C# material online, if prefer another source, go ahead and use it. Make sure it covers all the material in this tutorial.

Feel free to suggest new material on Discord, I will help in reviewing it.

[https://www.youtube.com/watch?v=GhQdlIFylQ8](https://www.youtube.com/watch?v=GhQdlIFylQ8)

## Intro to PowerShell

[https://www.youtube.com/watch?v=TUNNmVeyjW0](https://www.youtube.com/watch?v=TUNNmVeyjW0)

## Exercism.io - Optional

[Exercism](https://exercism.io) is a great resource for exercises in many languages. Sign up for the C# track and practice as many problems as possible.

Your Mentor will review your progress on exercism.

## The NuGET package manager

NuGet is a package management system for dotNET. The following videos explain what NuGet is and how to install and use it.

#### Aim

By the end of this section you should be able to install dotNET packages with NuGet. The upcoming assignment requires you to install packages to read CSV files and create plots.

[https://www.youtube.com/watch?v=WW3bO1lNDmo](https://www.youtube.com/watch?v=WW3bO1lNDmo)

## Data Project 1: Company Master

In this project, you will build a simple command-line application that will read in a CSV file, do some aggregation/filtering/grouping functions and print out the results in table format.

#### Source Data

Your source data will is the company registration data for the state of Maharashtra, from data.gov.in, the Government of India's open data platform.

Download the [Company Master Data of Maharashtra](https://data.gov.in/catalog/company-master-data) in CSV format.

#### Output

For each problem print the result in table format on the console. Use `ConsoleTables` package to print nicely formatted tables.

#### NuGet packages

One of the aims of this project is to familiarize yourself with the NuGet packaging system. The following packages are recommended, though alternatives to the following can also be used.

1. CsvHelper - Helps parsing your CSV files.
2. ConsoleTables - Helps to print good-looking tables on the console.

### Problems

#### 1. Count by `Authorized Cap`

Calculate the number of companies whose "Authorized Cap" falls in the following intervals  ...

  1. <= 1L
  2. 1L to 10L
  3. 10L to 1Cr
  4. 1Cr to 10Cr
  5. \> 10Cr

Print out the result of your calculation in table format using `ConsoleTables`.

The end result should look something like this ...

```text
 ------------------------
 | Bin         | Counts |
 ------------------------
 | <= 1L       | 20440  |
 ------------------------
 | 1L to 10L   | 125893 |
 ------------------------
 | 10L to 1Cr  | 50696  |
 ------------------------
 | 1Cr to 10Cr | 16323  |
 ------------------------
 | >10Cr       | 1844   |
 ------------------------

 Count: 5
```

#### 2. Company Registration by Year (From 2000 to 2019)

From the column DATE_OF_REGISTRAION `parse` out the registration year. Using this piece of data, calculate the number of company registrations per year. Print out the result of your calculation in table format using `ConsoleTables`.

#### 3. Company Registration by principal business activity (for the year 2015)

In this problem filter only the records for the year 2015. Then count the number of company registration by "PRINCIPAL_BUSINESS_ACTIVITY" and print them out in table format, similar to the previous tables.

#### 4. Grouped aggregation

For this problem, count the number of companies, grouped on both the year and "Principal Business Activity".
Also, restrict the years to 2000-2019.

The output should look like this ...

```text
 --------------------------------------------------------------------------------------------------------------------------------------------
 | Principal Business Activity                                                                                                     | Counts |
 --------------------------------------------------------------------------------------------------------------------------------------------
 | 2000                                                                                                                            |        |
 --------------------------------------------------------------------------------------------------------------------------------------------
 | Agriculture, hunting and related service activities                                                                             | 70     |
 --------------------------------------------------------------------------------------------------------------------------------------------
 | Forestry, logging and related service activities                                                                                | 6      |
 --------------------------------------------------------------------------------------------------------------------------------------------
 | Manufacture of food products and beverages                                                                                      | 92     |
 --------------------------------------------------------------------------------------------------------------------------------------------
 | Manufacture of chemicals and chemical products                                                                                  | 67     |
 --------------------------------------------------------------------------------------------------------------------------------------------
 | Manufacture of basic metals                                                                                                     | 35     |
 --------------------------------------------------------------------------------------------------------------------------------------------
 | Wholesale trade and commission trade, except of motor vehicles and motorcycles                                                  | 418    |
 --------------------------------------------------------------------------------------------------------------------------------------------
 | Financial intermediation                                                                                                        | 84     |
```

#### Submission

When you are done with the project submit the URL of github repository.

**NOTE** your repository should have a README.md file with instructions to run your project.


