# Zulu Bank Data Normalization and Database Integration
 
This repository contains a Python script for normalizing a denormalized dataset from Zulu Bank and integrating it into a PostgreSQL database. The script performs data transformation, normalization, and loading into a structured database schema.

## Overview
The script performs the following tasks:

1. Data Normalization:

   - Converts the dataset into 1NF, 2NF, and 3NF.
   - Splits FullName into first_name and last_name.
   - Creates separate tables for customer, accounts, transactions, and loans.
   - Further normalize the date table.

2. Database Integration:

   - Creates a PostgreSQL database named zulu_bank.
   - Defines a schema (zulu_bank_db) and tables for the normalized data.
   - Loads the normalized data into the respective tables.

3. Data Warehousing:

   + Generates dimension and fact tables for transactional and loan data.
   + Saves the data warehouse tables to CSV files (because at this stage, there's no warehouse I'm working with).

## Key Features
  + **Data Normalization:** Transforms raw data into a structured format.
  + **PostgreSQL Integration:** Automates database creation, schema definition, and data loading.
  + **Data Warehousing:** Prepares data for analytical queries with dimension and fact tables.

### Repository Contents
  + ERDs: Entity-Relationship Diagrams are included in the repository.
  + Datasets: The raw and processed datasets are stored in the Dataset folder.
  + Script: The main Python script for data normalization and database integration.

#### Prerequisites
  - Python 3.x
  - *Libraries:* pandas, psycopg2
  - *DB:* PostgreSQL installed and running locally.

**_For any questions or issues, please open an issue in the repository. Contributions are welcome! Thank you!!!_**
