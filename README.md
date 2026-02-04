# Customer Segmentation using KMeans Clustering

## Overview
This project performs **customer segmentation** using the **KMeans clustering algorithm** on the Mall Customer Segmentation dataset.  
The goal is to group customers based on their **annual income** and **spending behavior** to help businesses understand customer patterns and make data-driven decisions.

---

## Dataset
**Mall Customer Segmentation Dataset (Kaggle)**

### Features Used
- Annual Income (k$)
- Spending Score (1–100)

### Dropped Column
- CustomerID  
  (Identifier only, does not contribute to clustering)

---

## Tools & Technologies
- Python  
- Pandas  
- Scikit-learn  
- Matplotlib  

---

## Project Workflow

### 1. Data Loading & Exploration
- Loaded the dataset using Pandas
- Inspected data structure, summary statistics, and data types
- Verified absence of missing values

---

### 2. Data Preprocessing
- Removed irrelevant identifier column
- Selected relevant numerical features
- Applied **StandardScaler** to normalize features

**Why scaling is important:**  
KMeans is distance-based. Without scaling, features with larger ranges dominate cluster formation.

---

### 3. Finding Optimal Number of Clusters
- Applied KMeans for multiple values of K (1–10)
- Calculated inertia for each K
- Used the **Elbow Method** to identify the optimal number of clusters

---

### 4. Model Training
- Trained final KMeans model with optimal K
- Assigned cluster labels to each customer

---

### 5. Visualization
- Visualized clusters using a scatter plot:
  - X-axis: Annual Income
  - Y-axis: Spending Score
- Distinct colors represent different customer segments

---

### 6. Output
- Added cluster labels to the dataset
- Saved the segmented dataset as:

Mall_Customers_Segmented.csv

### Author 

Rushita Bhosale 
