# E-Commerce-Behavior-Analysis

We use a dataset of multicategory online stores to perform Exploratory Data Analysis and Predictive Modeling. Each row of the dataset is a transaction, indicating whether the user purchased the item at the end of the user journey. The analysis was performed by utilizing PySpark, AWS S3 and Databricks to produce efficient data processing workflow and drawing actionable insights for online stores to optimize their marketing strategies. This project is about consumer behavior analysis. Consumer behavior analysis is a data-driven observation of online consumers and how they interact with the company; in this project, we have tried to understand and analyze how users interact with online stores.


Business Questions: 
1. What is the most consumed product?
2. What is the most consumed category of all?
3. What are the top 5 brands that generate the most revenue?
4. What is the conversion rate of all customers for the brands?
5. Based on the given attributes in the dataset, how confident can we be in the prediction of  whether the users will purchase the product?


We use Databricks to connect our dataset stored in AWS S3 buckets to the analysis platform.

First, create a new user in AWS IAM and then set up the user to have full access to AWS S3. The reason to do this is because we need a user with credentials to mount S3 bucket to our notebook in Databricks and this user provides the credentials needed.

We created a user in AWS IAM called “connectionnew” and set the permission of this user to possess the full access to AWS S3.

With the access key of this user, we are allowed to connect from Databricks to our data stored in AWS S3 buckets.

We created a S3 bucket called “ecommercedatabudt737” and uploaded all csv files into this bucket and we used the data path from this bucket in Databricks to read these data to perform predictive analysis.
