# Customer Segmentation Based on Number of Products and Canceled Orders

Overview

This project aims to segment customers based on their purchasing behavior, specifically focusing on the number of products purchased and the number of canceled orders. Customer segmentation helps businesses identify different customer groups and tailor their strategies for personalized marketing, customer retention, and operational efficiency.

Two clustering techniques, KMeans Clustering and Gaussian Mixture Model (GMM) Clustering, are applied to identify distinct customer groups. The results are visualized using various plots, including pair plots, violin plots, and a correlation heatmap, to better understand customer behavior patterns.

Workflow
1. Data Loading and Cleaning
The dataset is loaded from a CSV file using pandas.
Duplicate rows are identified and removed to ensure data consistency.
Categorical and numerical columns are separated for further analysis.
2. Handling Missing Values
Missing values in the dataset are checked.
Rows with missing values in critical fields, such as CustomerID, are dropped to avoid incorrect segmentation.
3. Customer-Level Aggregation
Customer-level aggregation is performed to derive meaningful insights.
The number of unique products purchased by each customer is counted.
The number of canceled orders is identified and recorded for each customer.
4. Exploratory Data Analysis (EDA)
A correlation heatmap is generated to analyze the relationships between variables, helping identify significant features for clustering.
5. KMeans Clustering
The optimal number of clusters (k) is determined using the Elbow Method, which plots the Within-Cluster Sum of Squares (WCSS) against different values of k.
KMeans clustering is applied to group customers based on their numerical features.
The results are visualized using:
Pair Plots: To examine how different customer clusters are distributed in a multi-dimensional space.
Violin Plots: To analyze the distribution of numeric features within each cluster.
6. Gaussian Mixture Model (GMM) Clustering
The Gaussian Mixture Model (GMM), a probabilistic clustering technique, is applied to segment customers.
The Bayesian Information Criterion (BIC) and Akaike Information Criterion (AIC) scores are calculated for different numbers of components to determine the optimal number of clusters.
The segmentation results are visualized using violin plots to understand how each cluster differs in terms of the number of products purchased and canceled orders.

Results and Insights

The KMeans and GMM clustering results provide a deeper understanding of customer behavior.
The insights from the clusters can help businesses identify high-value customers, those with frequent order cancellations, and those with a diverse purchase history.
The findings can be used for personalized marketing strategies, customer retention efforts, and order fulfillment optimizations.

Technologies Used

Python (for data analysis and clustering)
pandas, NumPy (for data manipulation and preprocessing)
scikit-learn (for KMeans and GMM clustering)
matplotlib, seaborn (for data visualization)
