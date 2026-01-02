## Customer Segmentation using K-Means
### Project Overview

* This project focuses on customer segmentation using transactional retail data.
The goal is to group customers based on their purchasing behavior to help businesses understand customer value, loyalty, and churn risk.

### Problem Statement

* Businesses often treat all customers the same, which leads to:

* Inefficient marketing

* Poor retention strategies

* Revenue loss

* This project solves that by segmenting customers based on Recency, Frequency, and Monetary (RFM) metrics.

### Dataset

* Source: Superstore Sales Dataset

* Granularity: Transaction-level order data

Key Features Used:

* Sales

* Profit

* Order Frequency

* Discount

* Order Date

### Approach
1. Data Preprocessing

* Handled encoding issues (latin1)

* Converted order dates to datetime

* Aggregated transaction data to customer level

2️. Feature Engineering (RFM)

* Recency: Days since last purchase

* Frequency: Number of orders per customer

* Monetary: Total sales and profit per customer

3️. Scaling

* Applied feature scaling to normalize values before clustering

4️. Clustering

* Used K-Means Clustering

* Selected optimal number of clusters using the Elbow Method

* Assigned cluster labels to each customer

5️. Cluster Analysis

* Analyzed average behavior of each cluster

* Identified high-value, loyal, discount-sensitive, and at-risk customers

### Key Insights

* High discounts often correlate with lower profitability

* A small segment of customers contributes to most revenue

* Inactive customers can be clearly identified using recency

### Technologies Used

* Python

* Pandas, NumPy

* Scikit-learn

* Matplotlib, Seaborn

* Jupyter Notebook

### Business Impact

* Helps target high-value customers

* Identifies churn-risk segments

* Enables personalized marketing strategies
