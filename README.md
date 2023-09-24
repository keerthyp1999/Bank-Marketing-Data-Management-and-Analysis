## Title
**Bank Marketing Data Management and Analysis - Design and Optimization**
![image](https://github.com/keerthyp1999/Bank-Marketing-Data-Management-and-Analysis/assets/143935705/a65b9ba4-422a-4613-9670-41a6f712482e)
## Problem Statement
Banking institutions aim to identify potential term deposit subscribers effectively. This requires analyzing customer factors like age, income, credit history, and education to create profiles and detect behavior patterns. Excel files are commonly used for this, have limitations: handling large data volumes, security, and manual processes, hampering decision-making
## Proposed Solution
Banking institutions can solve Excel's limitations by transitioning to a secure database system. This involves designing a structured schema, ensuring secure data storage, implementing regular backups, and using advanced analysis tools for customer insights. By tailoring marketing efforts based on this data, institutions can increase the likelihood of converting potential customers into subscribers.
## Target Users
Marketing team - Uses database to identify potential customers based on demographics and transaction history.

Sales team -Uses database to track customer interactions and feedback.

Customer service team- Uses database to provide personalized support.

Management team Uses database to monitor success of campaign and make data-driven decisions on future product offerings.

IT professionals or data analysts -Ensure database is running efficiently and securely, and update and maintain database as necessary.
## Dataset 
The Bank Marketing Data is taken from UCI Machine Learning Repository and below is the link to the data source:
[https://archive.ics.uci.edu/ml/datasets/bank+marketing]
This dataset contains information related to direct marketing campaigns conducted by a Portuguese banking institution. The primary objective is to predict whether a potential customer is likely to subscribe to a term deposit or not. To streamline the analysis, unnecessary columns have been removed, and the data has been organized into multiple tables based on attribute types mentioned in the data source link.
## Project Description
The project involves creating a database called 'bankmarketing' in **PostgreSQL** and designing tables within this database. The table design process involves identifying functional dependencies and applying normalization concepts, particularly BCNF (Boyce-Codd Normal Form), to minimize redundancy and organize data effectively. The result is a set of distinct tables: **client_campaign_details, client_lastcontact_details, client_job_details, client_details, client_loan_details, and client_socioeconomic_details.**

Once the tables are defined, data is loaded into the database using Python scripts. The project utilizes the **psycopg2 library** to establish a connection to the 'bankmarketing' database. CSV files containing the data are read using the pandas library and then loaded into their respective tables via the established database connection using psycopg2.

To ensure data integrity and functionality, thorough testing is conducted using various SQL queries, including data insertion, updating, deletion, selection, and the use of triggers where necessary.

To enhance data visualization and provide better insights, the project also includes data visualization using Tableau, offering a comprehensive view of the dataset.
## Application Development
We have developed a user-friendly dashboard for management to easily view client and campaign information using **Flask**. Our website displays table information by retrieving data from databases. Our primary objective is to simplify the query process for end-users without requiring manual connections to the remote database.
## Tools Used
Postgre sql - For creation of database 

Python( JUpyter Notebook) - For psycopg2 , pandas to connect to database and load data

Flask - For Web development
## Contributors
Keerthy Priya Vanam (University at Buffalo)

Sushmitha Yanamandala(University at Buffalo)

Sree Nandhini Kurusali(University at Buffalo)







