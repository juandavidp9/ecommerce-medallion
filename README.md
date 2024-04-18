# Azure Ecommerce Project: Medallion Architecture with Pyspark

ETL Project of an E-commerce Company data following the medallion architecture.

1. Azure Data Factory is used to move the data into Azure Data Lake Storage (ADLS) converting the files from csv to parquet and creating chunks of data.
2. Azure Databricks is used to created the tables in Databrick's Delta Lake transactional leyer: Bronze layer (raw data), Silver layer (cleaned, augmented) and Golden layer (business metrics).                           Pyspark is used for the data transformations. 
3. The data is finally stored in Delta Lake following the One Big Table modeling approach.

This diagram ilustrates the architecture:

![architecture](https://drive.google.com/uc?id=1a8GNFGXnQ24NmUT58mBfZebkIQ7dIDB0)
