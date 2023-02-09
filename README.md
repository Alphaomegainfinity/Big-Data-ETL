# Big-Data-ETL

Background

Many of Amazon's shoppers depend on product reviews to make a purchase. Amazon makes these datasets publicly available. They are quite large and can exceed the capacity of local machines. One dataset alone contains over 1.5 million rows; with over 40 datasets, data analysis can be very demanding on the average local computer. Using the ETL as the first goal, process completely in the cloud and upload a DataFrame to an RDS instancem. The second goal will be to use PySpark or SQL to perform a statistical analysis of selected data.

Extract two Amazon customer review datasets, transform each dataset into four DataFrames, and load the DataFrames into an RDS instance.

Instructions

Explore the Amazon Reviews Links to an external site.datasets and pick two datasets to perform ETL.

Rename each part_one_starter_code.ipynb file according to the dataset using. 

Extract the Data

Read in each dataset using the correct header and sep parameters.

Get the number of rows in each dataset.

Transform the Data

For each dataset use the schema.sql file located in the Resources folder to create the four DataFrames as follows:

Create the "review_id_df" DataFrame with the appropriate columns and data types.

Create the "products_df" DataFrame that drops the duplicates in the "product_id" and "product_title columns.

Create the "customers_df" DataFrame that groups the data on the "customer_id" by the number of times a customer reviewed a product.

Create the "vine_df" DataFrame that has the "review_id", "star_rating", "helpful_votes", "total_votes", and "vine" columns.

Load the Data into an RDS Instance

Export each DataFrame into the RDS instance to create four tables for each dataset.

NOTE
This process can take up to 10 minutes for each
