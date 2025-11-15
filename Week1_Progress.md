**Project Overview**
The goal of this project is to analyze the customer journey on an e-commerce website. The business is getting high website traffic, but very few users are completing their purchases.
The objective is to understand where users are dropping off in the funnel and to prepare data that will support building a Power BI dashboard in the next stages of the project.

**Dataset Used**
For this project, I generated my own medium-sized dataset using Python in Google Colab.
The dataset includes:
events_medium.csv (around 1200 event records)
orders_medium.csv
products_medium.csv
This dataset contains the following details:
User and session information
Multiple event types: Homepage, ProductView, AddToCart, CheckoutStarted, Purchase
Device types: Mobile, Desktop, Tablet
Traffic sources and marketing campaigns
Product categories and pricing
Order details and timestamps
The dataset is designed to reflect a realistic clickstream pattern, including high traffic and lower purchase conversions, and stronger drop-off for mobile users.

**Work Completed This Week**
**Generated dataset in Google Colab**
I wrote a Python script to create a synthetic clickstream dataset that matches the project requirements.
The dataset includes events, orders, and products with proper structure.

**Loaded data into Power BI**
I imported all three CSV files into Power BI and verified that the rows, columns, and data types were correct.

**Initial Data Cleaning**
Removed empty or unnecessary rows
Checked consistency of event names
Confirmed product IDs and order IDs were valid across tables
Ensured timestamp and numeric fields were properly formatted

**Prepared for Data Modeling**
I planned the star schema that will be created in Week 2.
The fact and dimension tables include events, orders, users, sessions, products, traffic, and date.

**Summary of Week 1**

During Week 1, I completed the dataset creation, imported the data into Power BI, performed basic cleaning, and prepared the structure for modeling. This completes the foundation needed for Week 2.
