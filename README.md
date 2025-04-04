# Data Analyst  
**Technical Skills: Power BI, SQL, AWS, Python**

My medium articles about data analysis, business tips and other stuff: https://medium.com/@douglasbittencourt

# Professional Experience

**STAFF do Brasil • https://www.staffdobrasil.com.br/site/ • (70 employees) - Data Analyst; Valinhos, São Paulo, BR |
Power BI, MS SQL Server, AWS (Nov 2023 - Now)**

• Migrated all the dashboards of the company from GoodData to Power BI, giving many visual improvements and improved
decision-making speed

• Created a data warehouse on AWS, migrating part of the on-premisses database to cloud, improving security, reduced
dashboard load times by 10% and reduced maintenance costs

**Cogna Educação • https://www.kroton.com.br/ • (36,000 employees) - Data Analyst; Valinhos, São Paulo, BR |
Python, Power BI, PostgreSQL, MS Excel, SAP (Sep 2022 - Nov 2023)**

• Worked at the financial department, following the whole student's journey looking for continuous improvement through QA

• Automated the messaging and billing system for students with late payment using Python, avoiding having to send it manually

• Data analysis and building Dashboards using SQL and Power BI, to generate insights for managerial decision making.

**Elettromec • https://elettromec.com.br/ • (182 employees) - Junior Market Intelligence Analyst; Valinhos, São Paulo, BR |
Python, Power BI, SQL Server, MS Excel (Oct 2021 - Sep 2022)**

• Supported the sales team with reports, presentations, and dashboards using Power BI, which enhanced productivity and sales
insights.

• Automated routines using Python, helping to reduce operational work time.

• Conducted data extraction, storage, and analysis using MS Excel, SQL, and MS Access. Performed market and competitor
studies to identify opportunities.

# Education

Associate Degree in Software Analysis and Development (2020 - 2022) | **UNIP - Campinas, São Paulo, BR**

Graduate Course in Neuromarketing · (2016 - 2017) | **INOVA BUSINESS SCHOOL - Campinas, São Paulo, BR**

Degree in Business Administration with a concentration in Marketing (2012 - 2016) | **ESAMC - Campinas, São Paulo, BR**

# Projects

## Geocoding
### I made a script in Python for geocoding using Google Maps API - https://github.com/doougbr/Geocoding-Script

![image](https://github.com/user-attachments/assets/4cdda19d-2640-4844-a8f9-278314dad42a)


## **Perfume Market Analysis for Data Portfolio**
### I made this project to demonstrate knowledge in using the tools throughout the entire data pipeline creation process, up to delivering a final report in the form of a dashboard.
### One of my passions is perfumery, so I decided to dive into a database with perfume listings sourced from eBay to analise it and take valuables insights from it

**Tools:** Python (Pandas, Google Cloud and native libraries), Google Cloud Storage, BigQuery, Power BI, GitHub

**Processes:** ETL, Data Ingestion Automation, API Consumption, Dashboard Creation

**Steps:**

1. Download the database (via API)
2. Process data using Python and automate the upload to the GCS bucket
3. Create the dataset and tables in BigQuery
4. Consume data from BigQuery using Power BI and create a dashboard

# **Process Breakdown:**

First, I installed the Kaggle library

`pip install kaggle`

To use the API, it's necessary to create a folder called `.kaggle` in your home directory and save the JSON with the key there.

![image](https://github.com/user-attachments/assets/a0760f0c-68a3-445e-a27b-7eef648ee0fe)

The official API documentation shows how to query datasets.

![image](https://github.com/user-attachments/assets/258fc368-738b-422a-b9d6-cbf1e12eb6a2)

For uploading to GCS, I installed the library:

`pip install google-cloud-storage`

I then created a simple Python script that transforms the table into a dataframe, saves a Parquet file, and automatically uploads it to a bucket in Google Storage. The choice of Parquet was due to its excellent format with very reduced size and the ability to maintain metadata.


![image](https://github.com/user-attachments/assets/16599064-dcd2-42db-a3bb-22d9927611af)

I uploaded another similar dataset, but in CSV, to show the size difference between the files.

![image](https://github.com/user-attachments/assets/39f0d117-f534-4c97-87bc-a0703a18ddc3)

Next, I created a dataset and a table with the data in BigQuery, reading from the previously created bucket.

![image](https://github.com/user-attachments/assets/4935352e-2091-4bd5-933a-1508592a2bbc)

I ran a basic query to validate the table.

![image](https://github.com/user-attachments/assets/b19ea871-2451-45db-8979-0108045df878)

After that, I made the connection in Power BI with BigQuery.

![image](https://github.com/user-attachments/assets/645b0cb0-a5b4-4583-b56e-d6bc506bcdb7)


I made some transformations in Power Query, such as merging the datasets and separating the location by city, state, and country.

![image](https://github.com/user-attachments/assets/af8992c6-0d37-4e73-bff4-72499f7d7535)

Finally, I created a Power BI dashboard with excellent performance, using only native visuals and following good design practices, such as a clean layout, few color variations, contrast, and consistency.

![image](https://github.com/user-attachments/assets/608578c9-94dd-494b-89f3-6e74663b5809)

Lastly, I committed the project files to GitHub for version control.

![image](https://github.com/user-attachments/assets/eb2b8d97-913d-4579-8191-f7b36170158f)


