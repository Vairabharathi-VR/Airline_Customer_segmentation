# Airline_Customer_segmentation using KMeans Clustering

## Definition: KMeans Clustering

KMeans clustering is a partitioning method that divides a dataset into 'k' distinct, non-overlapping subsets (clusters). It is an unsupervised machine learning algorithm used for classification and segmentation of data points based on their similarity.

## Project Overview

### Dataset Description

The dataset consists of customer information with various attributes such as balance, miles earned with different credit cards, bonus miles, flight miles, and days since enrollment. The goal is to perform customer segmentation using the KMeans clustering algorithm to identify distinct groups of customers.

### Column Descriptions

- **ID**: Unique ID
- **Balance**: Number of miles eligible for award travel
- **Qual_miles**: Number of miles counted as qualifying for Topflight status
- **cc1_miles, cc2_miles, cc3_miles**: Miles earned with credit cards (categorized)
- **Bonus_miles**: Number of miles earned from non-flight bonus transactions
- **Bonus_trans**: Number of non-flight bonus transactions
- **Flight_miles_12mo**: Number of flight miles in the past 12 months
- **Flight_trans_12**: Number of flight transactions in the past 12 months
- **Days_since_enroll**: Number of days since enrolled in the flyer program
- **Award**: Whether the person had an award flight (free flight) or not

## Methodology

1. **Data Exploration and Preprocessing:**
    - Imported necessary packages
    - Checked data information (no null values)
    - Explored basic statistics of the data using describe
    - Dropped the 'ID' column as it is unique and not relevant for analysis

2. **Exploratory Data Analysis (EDA):**
    - Checked the distribution of categories for 'cc1_miles', 'cc2_miles', 'cc3_miles'
    - Explored correlation using a heatmap
    - Visualized the distribution of features with a pair plot

3. **KMeans Clustering:**
    - Utilized the Elbow Method to determine the optimal number of clusters (k=4)
    - Applied KMeans clustering with k=4
    - Added the 'Cluster' column to the dataset

4. **Visualization:**
    - Explored the distribution of clusters using a scatter plot (Balance vs. Days_since_enroll)
    
## Results

The KMeans clustering algorithm successfully segmented customers into four distinct clusters. The scatter plot revealed patterns in customer segmentation based on balance and days since enrollment. Further analysis and targeted strategies can be implemented for each customer cluster.

## Conclusion

The application of KMeans clustering provides valuable insights into customer segmentation, allowing businesses to tailor their marketing and service strategies for different customer groups. Understanding customer behavior and preferences is crucial for enhancing customer satisfaction and optimizing business outcomes.

