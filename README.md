# Customer Segmentation using K-Means Clustering

An Unsupervised Machine Learning project that applies **K-Means Clustering** to group retail customers based on their demographic and spending behaviour. The project explores customer purchasing patterns and identifies meaningful segments that can support data-driven marketing strategies and customer engagement.

## Project Overview

Understanding customer behaviour is important for businesses that want to improve customer experience, design targeted marketing campaigns, and build effective retention strategies.

In this project, K-Means Clustering is used to identify groups of customers with similar characteristics. By analyzing features such as age, annual income, and spending score, the project demonstrates how unsupervised learning can uncover patterns in customer data without requiring predefined labels.

## Objectives

- Explore customer demographic and spending patterns.
- Perform exploratory data analysis (EDA) to understand the dataset.
- Prepare numerical features for distance-based clustering.
- Apply the Elbow Method to help select an appropriate number of clusters.
- Implement K-Means Clustering to group customers.
- Interpret customer segments and understand their potential business applications.

## Dataset

The project uses the `Customers-Segmentation.csv` dataset.

The dataset contains customer information used to explore demographic and spending behaviour.

Key features discussed in the project include:

- **Age:** Customer's age.
- **Annual Income:** Customer's annual income.
- **Spending Score:** A score representing the customer's spending behaviour.

The selected features are used to identify similarities and differences between customers.

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

EDA is performed to understand the dataset before applying the clustering algorithm.

The analysis includes:

- Examining the dataset structure and basic statistics.
- Understanding the distributions of customer age, annual income, and spending score.
- Exploring relationships between numerical features.
- Using visualizations to identify patterns and potential customer groups.

### 2. Data Preprocessing

Data preprocessing prepares the selected features for clustering.

**Feature Scaling**

K-Means relies on distance calculations. Features with larger numerical ranges can dominate these calculations.

`StandardScaler` is used in the existing project description to standardize numerical features and make them more comparable.

### 3. Selecting the Number of Clusters — Elbow Method

Choosing the number of clusters is an important step in K-Means.

The Elbow Method evaluates different values of K by calculating the **Within-Cluster Sum of Squares (WCSS)**.

The WCSS measures the sum of squared distances between data points and their assigned cluster centroids.

The value of K is selected by examining the Elbow Curve and identifying the point where the reduction in WCSS begins to slow down.

### 4. K-Means Clustering

K-Means is an unsupervised learning algorithm that divides data points into K clusters.

The general process is:

1. Select the number of clusters (K).
2. Initialize cluster centroids.
3. Assign each customer to the nearest centroid.
4. Recalculate the centroids based on assigned customers.
5. Repeat the assignment and update steps until the clusters converge.

The existing project description specifies K-Means++ initialization and Euclidean distance for clustering.

### 5. Customer Segment Interpretation

After clustering, the resulting groups can be interpreted using customer income and spending behaviour.

Examples of possible customer segments include:

| Segment | Customer Characteristics | Potential Business Strategy |
|---|---|---|
| Premium Customers | High income, high spending | Loyalty programs and premium offers |
| Value Seekers | Low income, high spending | Personalized discounts and retention campaigns |
| Conservative Customers | High income, low spending | Targeted promotions and engagement |
| Standard Customers | Moderate income and spending | General marketing campaigns |

*Note: These are illustrative segment interpretations. Actual segment names and characteristics should be assigned after examining the clustering results.*

## Technologies Used

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Machine Learning:** Scikit-learn
- **Data Visualization:** Matplotlib, Seaborn
- **Development Environment:** Jupyter Notebook

## Repository Structure

```text
Customer-Segmentation-KMeans/
│
├── Customer Segmentation using K-Means Clustering.ipynb
├── Customers-Segmentation.csv
└── README.md
```

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/mani787060/Customer-Segmentation-KMeans.git
cd Customer-Segmentation-KMeans
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

Activate it on macOS/Linux:

```bash
source .venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install numpy pandas scikit-learn matplotlib seaborn jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

`Customer Segmentation using K-Means Clustering.ipynb`

Run the notebook cells sequentially.

## Key Learning Outcomes

Through this project, the following concepts are explored:

- Fundamentals of Unsupervised Machine Learning.
- Exploratory Data Analysis and data visualization.
- Feature scaling and preprocessing.
- Distance-based clustering algorithms.
- K-Means Clustering and centroid-based grouping.
- Selecting cluster counts using the Elbow Method.
- Interpreting clusters for practical business applications.

## Potential Applications

Customer segmentation can help businesses:

- Identify valuable customer groups.
- Develop targeted marketing campaigns.
- Improve customer retention strategies.
- Personalize offers and recommendations.
- Understand differences in customer spending behaviour.

## Future Improvements

Potential extensions include:

- Evaluating clustering quality using the Silhouette Score.
- Comparing K-Means with Hierarchical Clustering and DBSCAN.
- Applying PCA to visualize high-dimensional customer data.
- Developing an interactive customer segmentation dashboard.
- Exploring additional customer features for more meaningful segments.
