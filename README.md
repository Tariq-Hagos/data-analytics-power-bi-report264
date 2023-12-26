﻿# data-analytics-power-bi-report264
# Power BI Project Documentation

## Overview

This Power BI project involves importing and transforming data from different sources to create a comprehensive and insightful report. The project comprises four main tasks: importing the Orders table, cleaning the Products table, importing the Stores table, and importing customer data.

## Task 1: Orders Table

### Importing Orders_powerbi Table

- Connected to Azure SQL Database using the following credentials:
  - Server Name: `my-server-maya.database.windows.net`
  - Database Name: `orders_db`
  - Username: `******`
  - Password: `*******`
- Imported the `orders_powerbi` table using the Import option in Power BI.

### Cleaning and Transforming Orders Table

1. Deleted the column named [Card Number] for data privacy.
2. Used the Split Column feature to separate [Order Date] and [Shipping Date] into date and time components.
3. Filtered out and removed rows with missing or null values in the [Order Date] column.
4. Renamed columns to align with Power BI naming conventions.

## Task 2: Products Table

### Importing Products.csv

- Downloaded the `Products.csv` file.
- Used Power BI's Get Data option to import the file into the project.
- Used Remove Duplicates on the `product_code` column.

### Cleaning and Transforming Products Table

1. Used Column From Examples to generate new columns for weight values and units.
2. Replaced blank entries in the units column with "kg."
3. Converted the data type of the values column to decimal.
4. Replaced any conversion errors with the number 1.
5. Created a new calculated column for weight in kilograms.
6. Deleted unnecessary columns.
7. Renamed columns to adhere to Power BI naming conventions.

## Task 3: Stores Table

### Importing Stores Table from Azure Blob Storage

- Connected to Azure Blob Storage using the provided credentials.
  - Account Name: `powerbistorage2`
  - Account Key: `*****************************`
  - Container Name: `data-analytics`
- Imported the Stores table.
- Renamed columns to align with Power BI naming conventions.

## Task 4: Customers Data

### Importing Customers Folder

- Downloaded and unzipped the `Customers.zip` file.
- Used Power BI's Get Data option with the Folder data connector to import the Customers folder.
- Created a Full Name column by combining [First Name] and [Last Name].
- Deleted unused columns and renamed remaining columns.

## Documentation of Achievements

- Detailed the methods used to import data from different sources.
- Documented the transformations performed on each table.
- Saved the latest Power BI `.pbix` file and uploaded it to the GitHub repository.
