# Querying Spark Tables Using SQL Queries

SQL Server can't read Spark/Hive Database directly, and Synapse Analytics can transform Spark database into replicated database which can be support with tranditional SQL Queries. It doesn't require any code or backend support for using Synapse Analytics.
Below image is Synapse Analytics Pipeline.

![image](https://user-images.githubusercontent.com/71728495/150847606-f095863c-9ae2-4a34-a9b2-e18329688f58.png)

# Demo read Parquet file with SQL Queries

In this demo, it will read a parquet format file with using SQL Queries. 
 
## 1) Create a Synapse workspace in the Azure portal

![image](https://user-images.githubusercontent.com/71728495/150852749-f843dd95-527c-4a05-b968-eb8f5f92e631.png)

## 2) Open Synapse Studio
Since we don't have SQL connection from local, we will launch Synapse Studio for demo purpose.

![image](https://user-images.githubusercontent.com/71728495/150853438-71a327f9-bbb6-4c12-add0-4e1c9017182f.png)

## 3) Place sample data into datalake service

Use a 100k row sample data of NYX Taxi Cab data.

Download link: https://azuresynapsestorage.blob.core.windows.net/sampledata/NYCTaxiSmall/NYCTripSmall.parquet

Place in Azure Data Lake Storage Gen2

![image](https://user-images.githubusercontent.com/71728495/150854063-16a78b98-114e-4564-a873-a17660fe36cb.png)

## 4) Run Synapse Studio
Access develop mode, you can use different method such as Notebook (Python) or SQL query

![image](https://user-images.githubusercontent.com/71728495/150854632-cd30caa3-672c-4fc8-ab6d-3e51cd6c4bea.png)

## 5) The Built-in serverless SQL pool
Severless SQL pools let you load Spark/Hive table (NoSQL database) using SQL Queries.

![image](https://user-images.githubusercontent.com/71728495/150854968-2e55a870-157b-4edf-96ec-d10c4c2c29cb.png)



