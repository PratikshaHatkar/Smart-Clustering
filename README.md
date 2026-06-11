# Smart Customer Segmentation using Machine Learning

## Project Overview

This project focuses on **customer segmentation** using unsupervised machine learning techniques. The objective is to identify distinct groups of customers based on their demographics, purchasing behavior, and engagement patterns. These insights can help businesses design targeted marketing campaigns and improve customer relationship strategies.

---

## Problem Statement

Businesses often have a large customer base with diverse purchasing behaviors. Treating all customers the same can lead to ineffective marketing and reduced profitability.

The goal of this project is to:

- Analyze customer data.
- Discover hidden patterns in customer behavior.
- Segment customers into meaningful groups using clustering algorithms.
- Interpret the characteristics of each customer segment.

---

## Dataset

The dataset contains customer information such as:

- Demographic details
- Income levels
- Education status
- Marital status
- Customer tenure
- Product spending patterns
- Number of children at home
- Purchase behavior across different channels

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Kneed

---

## Project Workflow

### 1. Data Loading and Exploration

- Imported customer dataset.
- Examined dataset shape and structure.
- Checked for missing values.

---

### 2. Data Preprocessing

#### Missing Value Handling

- Filled missing values in the **Income** column using the median value.

#### Feature Engineering

Created new features including:

- **Age**
- **Customer_Tenure_Days**
- **Total_Spending**
- **Total_Children**

Grouped categorical variables:

- Education levels
- Living status

---

### 3. Feature Selection

Removed unnecessary columns such as:

- Customer ID
- Birth Year
- Marital Status
- Children-related original columns
- Customer joining date
- Individual spending columns after calculating total spending

---

### 4. Outlier Treatment

Removed extreme observations from:

- Age
- Income

to improve clustering performance.

---

### 5. Exploratory Data Analysis

Performed:

- Pair plots
- Correlation analysis
- Heatmap visualization

to understand relationships among features.

---

### 6. Encoding Categorical Variables

Applied **One-Hot Encoding** on:

- Education
- Living status

---

### 7. Feature Scaling

Used **StandardScaler** to standardize the data before clustering.

---

### 8. Dimensionality Reduction

Applied **Principal Component Analysis (PCA)** to reduce dimensionality and visualize customer groups effectively.

Visualizations included:

- 2D PCA plots
- 3D PCA plots

---

### 9. Finding Optimal Number of Clusters

Two approaches were used:

#### Elbow Method

- Computed Within Cluster Sum of Squares (WCSS).
- Used **KneeLocator** to identify the elbow point.

#### Silhouette Analysis

- Calculated silhouette scores for different values of K.
- Compared clustering quality across multiple cluster counts.

---

### 10. Customer Segmentation

Implemented two clustering algorithms:

#### K-Means Clustering

Used to partition customers into distinct groups.

#### Agglomerative Clustering

Applied hierarchical clustering using Ward linkage.

---

### 11. Cluster Analysis

Generated cluster profiles by analyzing average feature values within each cluster.

Visualized clusters using:

- Count plots
- Spending vs Income scatter plots

---

## Customer Segments Identified

The analysis identified four major customer groups:

### Cluster 0
- Moderate income customers.
- Moderate spending behavior.
- Price-sensitive segment.

### Cluster 1
- High income customers.
- High spending behavior.
- Premium customer segment.

### Cluster 2
- Low income customers.
- Low spending behavior.
- Highly price-sensitive customers.

### Cluster 3
- Moderate to high income customers.
- Selective spending behavior.
- Potential premium customers.

---

## Business Applications

The identified segments can be used for:

- Personalized marketing campaigns.
- Customer retention strategies.
- Product recommendation systems.
- Loyalty program design.
- Improving overall customer experience.

---

## Results

The project successfully segmented customers into meaningful groups, enabling businesses to better understand their customer base and make data-driven marketing decisions.
---
