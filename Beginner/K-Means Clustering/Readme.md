# Customer Segmentation using K-Means Clustering

This project performs customer segmentation using the K-Means clustering algorithm. The goal is to segment customers into different groups based on their demographic and purchasing behavior, which can be used to inform targeted marketing strategies.

## Project Overview

Customer segmentation is a key application in marketing that allows businesses to understand different customer groups and tailor their marketing strategies accordingly. This project aims to classify customers based on features such as age, annual income, and spending habits using K-Means clustering, an unsupervised machine learning algorithm.

## Dataset

The dataset used for this project is the **Mall Customers Dataset**, which includes information about customers such as:
- **CustomerID**: Unique identifier for each customer.
- **Gender**: Gender of the customer (Male/Female).
- **Age**: Age of the customer.
- **Annual Income (k$)**: Annual income of the customer in thousands of dollars.
- **Spending Score (1-100)**: Score assigned by the mall, representing the customer's spending behavior.

### Data Preprocessing
- Dropped the `CustomerID` column as it is not useful for clustering.
- Selected features for clustering: `Age`, `Annual Income (k$)`, and `Spending Score (1-100)`.
- Standardized the data to have a mean of 0 and standard deviation of 1.

## Project Steps

1. **Data Loading and Exploration**: Loaded the dataset and performed an initial exploration to understand its structure.
2. **Data Preprocessing**: Cleaned and standardized the data to prepare it for clustering.
3. **K-Means Clustering**:
   - Used the **Elbow Method** and **Silhouette Score** to determine the optimal number of clusters.
   - Chose **6 clusters** based on the analysis.
   - Applied the K-Means algorithm to segment the customers.
4. **Cluster Visualization**:
   - Visualized the clusters using **scatter plots**, **pair plots**, and a **heatmap** of cluster centers.
5. **Result Interpretation**:
   - Analyzed the characteristics of each cluster to draw insights and suggest targeted marketing strategies.

## Key Insights

- The clusters revealed distinct customer segments, such as **young high-income high spenders**, **older moderate-income average spenders**, and **middle-aged high-income low spenders**.
- These insights can help in creating personalized marketing strategies for each segment, such as loyalty programs for high spenders and budget-friendly promotions for low-income groups.

## Visualizations

The project includes several visualizations to help understand the clusters:
- **Scatter Plots**: Show relationships between pairs of features colored by cluster.
- **Pair Plot**: Provides a multi-dimensional view of the clusters.
- **Heatmap**: Visualizes the average feature values for each cluster, highlighting the differences in customer behavior.

## Installation

To run this project, ensure you have Python installed and the necessary libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
