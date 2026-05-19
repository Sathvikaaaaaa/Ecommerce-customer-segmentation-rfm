# E-Commerce Customer Segmentation using RFM and Clustering

## Project Overview

This project focuses on analyzing e-commerce transaction data to understand customer purchasing behavior and segment customers into meaningful groups using RFM Analysis and K-Means Clustering.

The goal of the project is to help the business improve customer retention, design targeted marketing campaigns, identify high-value customers, and support data-driven decision-making.

---

# Business Problem

The e-commerce company wants to better understand its customers and their purchasing behavior.

The company faces challenges such as:

* Identifying loyal and high-value customers
* Recognizing inactive or at-risk customers
* Improving customer retention
* Designing personalized marketing campaigns
* Increasing revenue through customer segmentation

To solve these problems, customer transaction data was analyzed using RFM metrics and clustering techniques.

---

# Dataset Source

Dataset provided as part of the Business Analytics Project assignment.

Source:
Google Drive Dataset Folder shared by the instructor.

Dataset Used:
Part 1 - E-Commerce Customer Segmentation using RFM and Clustering

---

# Dataset Description

The dataset contains transaction-level purchase records from an e-commerce business.

Each row represents a single product purchased within an invoice.

## Dataset Columns

* InvoiceNo → Unique invoice number
* StockCode → Unique product code
* Description → Product description
* Category → Product category
* Quantity → Number of units purchased
* InvoiceDate → Date and time of transaction
* UnitPrice → Price per unit
* CustomerID → Unique customer identifier
* Country → Country of customer
- InvoiceNo → Unique invoice number
- StockCode → Unique product code
- Description → Product description
- Category → Product category
- Quantity → Number of units purchased
- InvoiceDate → Date and time of transaction
- UnitPrice → Price per unit
- CustomerID → Unique customer identifier
- Country → Country of customer

---

# Tools and Libraries Used

## Programming Language

* Python

## Libraries

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn

## Development Environment

* VS Code
* Jupyter Notebook
* GitHub

---

# Steps Performed
- Python

## Libraries

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Development Environment

- VS Code
- Jupyter Notebook
- GitHub

---

# Project Workflow

1. Imported required libraries
2. Loaded the dataset
3. Performed data understanding
4. Cleaned missing and invalid data
5. Created revenue and customer-level features
6. Performed Exploratory Data Analysis (EDA)
7. Built RFM table
8. Scaled RFM features
9. Applied K-Means clustering
10. Interpreted customer segments
11. Generated business recommendations

---

# Data Cleaning Summary

The following cleaning steps were performed:

* Removed duplicate records
* Removed rows with missing CustomerID values
* Removed rows with missing product descriptions
* Removed rows with zero or negative quantities
* Removed rows with zero or negative unit prices
* Converted InvoiceDate column to datetime format
* Created Revenue column using Quantity × UnitPrice
- Removed duplicate records
- Removed rows with missing CustomerID values
- Removed rows with missing product descriptions
- Removed rows with zero or negative quantities
- Removed rows with zero or negative unit prices
- Converted InvoiceDate column to datetime format
- Created Revenue column using Quantity × UnitPrice

Final cleaned dataset contained 3848 rows.

---

# Feature Engineering Summary

Customer-level features were created from transaction-level data:

* Total Revenue
* Total Purchases
* Total Quantity Purchased
* Unique Products Purchased
* Average Order Value
* Customer Country

RFM metrics were also calculated:

* Recency → Days since last purchase
* Frequency → Number of purchases
* Monetary → Total customer spending
- Total Revenue
- Total Purchases
- Total Quantity Purchased
- Unique Products Purchased
- Average Order Value
- Customer Country

RFM metrics were also calculated:

- Recency → Days since last purchase
- Frequency → Number of purchases
- Monetary → Total customer spending

---

# Exploratory Data Analysis (EDA)

The following analyses were performed:

* Top countries by revenue
* Most sold products
* Highest revenue generating products
* Distribution of customer purchase frequency
* Distribution of average order value
* Outlier analysis for quantity, unit price, and revenue

## Key Insights

* Certain countries contributed significantly higher revenue compared to others.
* Some products were purchased frequently in high quantities.
* High-value products generated substantial revenue despite lower sales volume.
* Customer spending and purchase frequency showed noticeable variation.
* Outliers existed in quantity and revenue, indicating bulk or premium purchases.

---

# Clustering Approach
- Top countries by revenue
- Most sold products
- Distribution of customer purchase frequency
- Distribution of average order value
- Outlier analysis for quantity, unit price, and revenue

## Key Insights

- Certain countries contributed significantly higher revenue compared to others.
- Some products were purchased frequently in high quantities.
- High-value products generated substantial revenue despite lower sales volume.
- Customer spending and purchase frequency showed noticeable variation.
- Outliers existed in quantity and revenue, indicating bulk or premium purchases.

---

# Customer Segmentation using K-Means

K-Means clustering was applied using the RFM metrics.

## Steps Followed

1. Selected Recency, Frequency, and Monetary features
2. Standardized the features using StandardScaler
3. Used the Elbow Method to determine the optimal number of clusters
4. Applied K-Means clustering with 3 clusters
5. Assigned cluster labels to customers

---

# Cluster Interpretation

## Cluster 0 - Regular Customers

* Moderate spending and purchase frequency
* Stable customer segment
* Potential for upselling and personalized recommendations

## Cluster 1 - High Value Loyal Customers

* Highest frequency and monetary contribution
* Most valuable customer segment
* Important for long-term profitability

## Cluster 2 - Inactive or At-Risk Customers

* High recency with lower spending
* Customers have not purchased recently
* Higher risk of customer churn
- Moderate spending and purchase frequency
- Stable customer segment
- Potential for upselling and personalized recommendations

## Cluster 1 - High Value Loyal Customers

- Highest frequency and monetary contribution
- Most valuable customer segment
- Important for long-term profitability

## Cluster 2 - Inactive or At-Risk Customers

- High recency with lower spending
- Customers have not purchased recently
- Higher risk of customer churn

---

# Final Business Recommendations

* Provide loyalty rewards and exclusive offers to high-value customers.
* Launch personalized re-engagement campaigns for inactive customers.
* Use targeted recommendations to increase purchase frequency among regular customers.
* Focus marketing campaigns on high-revenue countries.
* Promote high-performing products using targeted advertising.
* Monitor declining customer activity and provide timely retention offers.
* Use customer segmentation to personalize email marketing campaigns.
- Provide loyalty rewards and exclusive offers to high-value customers.
- Launch personalized re-engagement campaigns for inactive customers.
- Use targeted recommendations to increase purchase frequency among regular customers.
- Focus marketing campaigns on high-revenue countries.
- Promote high-performing products using targeted advertising.
- Monitor declining customer activity and provide timely retention offers.
- Use customer segmentation to personalize email marketing campaigns.

---

# Project Outputs

The project repository contains:

* notebook.ipynb
* requirements.txt
* dataset_source.md
* outputs/customer_segments.csv
* README.md
- notebook.ipynb
- requirements.txt
- dataset_source.md
- outputs/customer_segments.csv
- README.md

---

# How to Run the Project

## Clone Repository

```bash
git clone https://github.com/Sathvikaaaaaa/Ecommerce-customer-segmentation-rfm.git
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Run Notebook

Open `notebook.ipynb` using Jupyter Notebook or VS Code and run all cells.

---

# Conclusion

This project successfully analyzed e-commerce customer behavior using RFM analysis and K-Means clustering.

The analysis identified different customer segments such as loyal customers, regular customers, and inactive customers. These insights can help businesses improve customer retention, personalize marketing strategies, and increase overall revenue using data-driven decision-making.
This project analyzed e-commerce customer purchasing behavior using RFM Analysis and K-Means Clustering.

Customer segmentation identified high-value, medium-value, and inactive customer groups based on recency, frequency, and monetary spending behavior.

The analysis provides valuable insights that can help businesses:

- Improve customer retention
- Personalize marketing campaigns
- Optimize customer engagement
- Increase long-term business revenue

Customer segmentation supports data-driven business decision-making and helps businesses better understand customer value.
