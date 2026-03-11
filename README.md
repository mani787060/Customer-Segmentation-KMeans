# Customer Segmentation using K-Means Clustering

## Executive Summary
This project applies **Unsupervised Machine Learning** to identify distinct customer segments within a retail dataset. By analyzing features like Annual Income and Spending Scores, the model uncovers hidden patterns that allow for data-driven marketing strategies and personalized customer engagement.

---

## The Data Science Pipeline

### 1. Exploratory Data Analysis (EDA)
* Distribution analysis of Age, Income, and Spending Score.
* Correlation heatmaps to identify relationships between features.

### 2. Data Preprocessing
* **Feature Scaling:** Implemented `StandardScaler` to ensure the K-Means distance-based calculations are not biased by varying feature magnitudes.
* **Dimensionality Check:** Selecting the most impactful features for clustering.

### 3. Model Optimization (The Elbow Method)
* Calculated **Within-Cluster Sum of Squares (WCSS)** for a range of $K$ values.
* Identified the "Elbow Point" to determine the mathematically optimal number of clusters, balancing model complexity with granularity.

### 4. K-Means Clustering
* Algorithm: K-Means++ initialization to avoid local optima.
* Clustering: Partitioning data into $K$ distinct groups based on Euclidean distance.

---

## Key Insights & Segments
The model typically identifies the following high-impact segments:
* **Target Group:** High income, high spending (Premium customers).
* **Value Seekers:** Low income, high spending (Potential for loyalty programs).
* **Conservative:** High income, low spending (Focus for targeted promotions).
* **Standard:** Mid-range income and spending.

---

## Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn
* **Visualization:** Matplotlib, Seaborn

---

## How to Use
1. Clone the repo: `git clone https://github.com/your-username/customer-segmentation-kmeans.git`
2. Install requirements: `pip install -r requirements.txt`
3. Open the Jupyter Notebook: `jupyter notebook customer_segmentation.ipynb`
