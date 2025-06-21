# Customer-Segmentation-using-Clustering 🧑‍🤝‍🧑

🎯 Aim
To identify distinct customer segments based on purchasing behavior using RFM (Recency, Frequency, Monetary) analysis. This segmentation helps an online retailer understand customer value and tailor marketing strategies effectively.

✅ Objectives
Perform Exploratory Data Analysis (EDA) on customer transaction data.

Create RFM features for each customer.

Clean and preprocess the dataset by handling missing values and outliers.

Standardize features for clustering.

Apply K-Means clustering to group customers based on purchasing patterns.

Identify optimal number of clusters using Elbow and Silhouette methods.

Interpret the resulting customer segments for business insights.

📊 Dataset Details
Source: https://www.kaggle.com/code/akramhussainkhan/time-series-analysis-for-retail-data/input

Total Records: 541,909 rows × 8 columns

Columns:

InvoiceNo, StockCode, Description, Quantity

InvoiceDate, UnitPrice, CustomerID, Country

Preprocessing Steps:

Removed rows with null CustomerID or Description

Added new features: Amount, Recency, Frequency, Monetary

Treated outliers in RFM features

Standardized data for clustering

🧰 Libraries & Packages Used
python
Copy
Edit
# Core Libraries
import numpy as np
import pandas as pd

# Visualization
import matplotlib.pyplot as plt
import seaborn as sns

# Date & Time
import datetime as dt

# Scikit-learn for Preprocessing & Clustering
from sklearn.preprocessing import StandardScaler
from sklearn.cluster import KMeans
from sklearn.metrics import silhouette_score
📈 Inferences & Conclusion
Best Number of Clusters: 3 (based on silhouette score and elbow method).

Cluster Insights:

Cluster 1: High-value customers with high transaction amounts and frequency — ideal for loyalty programs.

Cluster 0: Moderately active customers — potential for targeted marketing.

Cluster 2: Least active and infrequent buyers — less business impact, can be targeted with re-engagement offers.

K-Means clustering effectively segmented customers, aiding personalized marketing and improving customer relationship strategies.
