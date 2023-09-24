## Title
Bank Marketing Data Management and Analysis - Design and Optimization
![image](https://github.com/keerthyp1999/Bank-Marketing-Data-Management-and-Analysis/assets/143935705/a65b9ba4-422a-4613-9670-41a6f712482e)
## Problem Statement
Banking institutions need to effectively identify potential customers who are likely to subscribe to term deposits to increase their profitability. To do this, they need to analyze various factors such as age, income, credit history, and education of potential customers. This analysis can help banking institutions create customer profiles and identify patterns in customer behavior, which can inform targeted marketing and outreach strategies. The use of Excel files to store customer data can be limited to banking institutions. Excel files may not be able to handle the large volume of customer data that banking institutions collect, and they can become slow and inefficient. Excel files may also have limited security features, which can lead to insecure data storage. Moreover, working with Excel files can be a manual and time-consuming process, which can lead to slower decision-making.
## PROPOSED SOLUTION
Banking institutions can overcome the challenges posed by using Excel files by utilizing a database to securely store and manage customer data. Databases offer numerous benefits, such as the capability to efficiently handle a large volume of data, advanced querying and reporting capabilities, and enhanced security features like user authentication and access control. In addition, databases facilitate collaboration by enabling multiple users to work on data simultaneously, thereby streamlining the overall data management process.
To adopt a database system, the first step is to create a structured schema that can efficiently store customer data.
Stored customer data should be securely stored in the database and backed up regularly to prevent data loss. Advanced querying and reporting capabilities can then be utilized to analyze the stored data to gain valuable insights into customer behavior and preferences. This can help tailor marketing campaigns and improve customer service by customizing offers and promotions based on individual customer preferences and past interactions with the bank, increasing the chance of converting potential customers into subscribers.
## Target Users
Marketing team - Uses database to identify potential customers based on demographics and transaction history.

Sales team -Uses database to track customer interactions and feedback.

Customer service team- Uses database to provide personalized support.

Management team Uses database to monitor success of campaign and make data-driven decisions on future product offerings.

IT professionals or data analysts -Ensure database is running efficiently and securely, and update and maintain database as necessary.
## Dataset 
The Bank Marketing Data is taken from UCI Machine Learning Repository and below is the link to the data source:
[https://archive.ics.uci.edu/ml/datasets/bank+marketing]
This dataset pertains to the direct marketing campaigns of a Portuguese banking institution and can be used to predict whether a potential customer is likely to subscribe to a term deposit or not.Columns which are not necessary for the analysis are removed and the data is split into multiple tables based on the attribute types mentioned in the data source link. 
## Description
The database ‘bankmarketing’ is created in postgresql and then tables are created in the database. To design the tables , we have identified Functional Dependencies and  used normalization concepts like BCNF which helped to us to reduce redundancy and segregate tables properly into  different tables namely client_campaign_details, client_lastcontact_details,c.	client_job_details, client_details,client_loan_details,client_socioeconomic_details. 
Once the tables are created, the data is loaded to the database using python scripts. We used psycopg2 library to connect to bankmarketing database. The csv files are read using pandas library and are loaded to the tables through the connection established to the database using psycopg2 library. Once the data is loaded, it is tested using multiple sql queries which include data insert, update, delete, select and trigger queries. Optimization is done by creating indexes.
To get better view of the data , we have also visualized them in tableau.
## Application Development
We have developed a user-friendly dashboard for management to easily view client and campaign information using Flask. Our website displays table information by retrieving data from databases. Our primary objective is to simplify the query process for end-users without requiring manual connections to the remote database.






