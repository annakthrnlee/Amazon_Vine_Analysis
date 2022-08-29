# Amazon_Vine_Analysis
### Overview:
I was given access to 50 datasets and each one contained reviews of a specific product, all of which analyze Amazon reviews written by members of the paid Amazon Vine program. From the 50 datasets, I chose one (Automobiles) and used PySpark to perform an ETL process to extract the dataset, transform the data, connect it to an AWS RDS instance, and load the transformed data into pgAdmin. Then, I used SQL to determine if there was any bias toward favorable reviews from Vine members in your dataset. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

### Resources:
- PgAdmin 4
- Google Colab Notebooks
- SQL
- AWS (RDS)

##### What I did:
I used PySpark to extract, transform, and connect to my AWS RDS instance. Transformed the DataFrame into four separate DataFrames and uploaded them into the appropriate tables. Then, I ran the queries in pgAdmin to confirm that the data had been uploaded. Using Google Colab I imported PySpark Libraries and connected to Postgres to create the SQL tables and export the results.

### Results: 
After ensuring that the Amazon Review dataset was extracted as a DataFrame and transformed into four different DataFrames with the accurate columns, I filtered/created a new DataFrame. Here are my results:

- Total number of paid reviews: 82
- Total number of paid 5-star reviews: 33 (40.24%)
- Total number of unpaid reviews: 24742
- Total number of unpaid 5-star reviews: 12807 (51.76%)

<img width="796" alt="Screen Shot 2022-08-28 at 6 41 37 PM" src="https://user-images.githubusercontent.com/104043438/187102347-4d75dc6b-f834-4766-845e-11d80eb8d3ac.png">

