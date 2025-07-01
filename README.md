# Customer Segmentation using K-Means Clustering

This project demonstrates the application of **K-Means Clustering**, an unsupervised learning technique, to segment customers into meaningful groups based on their demographics and purchasing behavior. Using data visualization and multiple cluster evaluation methods, we identify optimal clusters to enable businesses to design personalized marketing strategies.

---

##  Overview

Customer segmentation is a powerful marketing strategy used to group customers based on shared characteristics. By identifying distinct customer segments, companies can tailor their services and promotional efforts, optimize resource allocation, and increase profitability.

This project uses **K-Means clustering**, a widely used algorithm for clustering unlabeled data. It divides the customer base into clusters based on features such as **age**, **annual income**, and **spending score**, enabling a deeper understanding of customer behavior.

---

## What is Customer Segmentation?

Customer segmentation is the process of dividing a customer base into groups that exhibit similar traits, such as age, gender, income, interests, and spending patterns. This helps businesses:
- Understand customer needs more precisely
- Tailor marketing campaigns to specific customer types
- Increase customer satisfaction and brand loyalty
- Reduce the risk of marketing investment by targeting the right groups

---

## What is the K-Means Algorithm?

**K-Means Clustering** partitions data into `k` distinct, non-overlapping subgroups (clusters), where each data point belongs to the cluster with the nearest mean (centroid). The algorithm works in the following steps:

1. Choose the number of clusters `k`.
2. Initialize `k` centroids randomly.
3. Assign each data point to the nearest centroid.
4. Recalculate the centroids as the mean of all assigned points.
5. Repeat steps 3–4 until the assignments no longer change (convergence).

---

## Dataset

- **Source:** [Mall Customer Segmentation Dataset on Kaggle](https://www.kaggle.com/nelakurthisudheer/mall-customer-segmentation)
- **Features:**
  - `CustomerID`: Unique customer ID
  - `Gender`: Male or Female
  - `Age`: Age of the customer
  - `Annual Income (k$)`: Income of the customer in thousands
  - `Spending Score (1–100)`: Score based on customer behavior and spending

---

##  Implementation Steps

### 1. **Data Exploration**
- Loaded and inspected data using R functions like `read.csv()`, `summary()`, and `str()`.
- Conducted initial statistical analysis and summary of age and income distributions.

### 2. **Visualizations**
Created multiple plots for exploratory analysis:
- **Bar Plot** and **Pie Chart** for gender distribution
- **Histogram** and **Box Plot** for Age, Income, and Spending Score
- **Density Plot** for income distribution

### 3. **K-Means Clustering**
- Selected relevant features: Age, Annual Income, Spending Score
- Applied K-Means algorithm using Euclidean distance
- Iteratively optimized cluster centroids

### 4. **Optimal Cluster Evaluation**
Used three common methods to determine optimal number of clusters:
- **Elbow Method**: Identified bend in the curve of intra-cluster variance
- **Silhouette Score**: Measured how similar a point is to its cluster
- **Gap Statistic**: Compared intra-cluster variation against null reference distribution

### 5. **Cluster Analysis**
- Visualized and interpreted customer clusters using PCA
- Derived behavioral insights from each cluster based on their characteristics

---

## Key Findings

- Clustered customers into **4 optimal segments** using Elbow and Silhouette methods.
- Observed clear separation between high spenders, low-income groups, and average consumers.
- Identified marketing strategies for each cluster, such as loyalty programs for high spenders or budget-friendly offers for low-income segments.

---

## 🛠 Technologies Used

- **Language:** Python
- **Packages:** `ggplot2`, `cluster`, `plotrix`, `purrr`, `gridExtra`
- **Techniques:** K-Means Clustering, PCA, Elbow Method, Silhouette Score, Gap Statistic




