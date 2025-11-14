# Mall Customer Segmentation using K-Means Clustering
This project applies the K-Means Clustering algorithm to segment mall customers based on their purchasing and income habits. The goal is to identify distinct customer groups for targeted marketing strategies.

## Dataset
Source: [Mall Customer Data](https://github.com/navyaprashanth/MallCustomerSegmentation_KMeansClustering/issues/1#issue-3624804304)
File: [Mall_Customers.csv](https://github.com/user-attachments/files/23544206/Mall_Customers.csv)

## Project Breakdown
### 1. Data loading and cleaning
We load the data using Pandas and perform a basic check for missing values.

### 2. Feature Selection
We isolate the two columns critical for clustering: Annual Income (column index 3) and Spending Score (column index 4).

### 3. Determining the Optimal Number of Clusters (K)
The Elbow Method is used to find the ideal number of clusters by minimizing the Within Cluster Sum of Squares (WCSS). We test K from 1 to 10.

### 4. Visualizing the Elbow Graph
The plot shows the point where the decrease in WCSS starts to slow down significantly (the "elbow" which I have marked with a red dot in the graph).
<img width="610" height="463" alt="Image" src="https://github.com/user-attachments/assets/71bae946-86e7-4bd1-a2a2-ed98df3c5e36" />
