# SmartCart

## E-commerce Customer Segmentation System

SmartCart is an **unsupervised machine learning project** focused on segmenting e-commerce customers based on their demographic and purchasing behavior.

The project applies data preprocessing, feature engineering, dimensionality reduction, and clustering techniques to identify meaningful customer groups from historical customer data.

## Project Overview

Customer segmentation helps businesses understand different types of customers and their purchasing patterns. In this project, customer data is processed and transformed into meaningful features before applying clustering algorithms.

The workflow includes:

* Data cleaning and preprocessing
* Feature engineering
* Categorical feature encoding
* Feature scaling
* Principal Component Analysis (PCA)
* Cluster evaluation using the Elbow Method and Silhouette Score
* Customer segmentation using K-Means Clustering
* Customer segmentation using Agglomerative Clustering
* Cluster analysis and interpretation

## Dataset

The project uses `smartcart_customers.csv`, containing customer demographic, household, and purchasing information.

The dataset contains approximately **2,240 customer records** with multiple attributes related to:

* Customer demographics
* Income
* Household composition
* Product spending
* Purchase behavior
* Campaign response

## Data Preparation

The dataset is prepared through several preprocessing steps:

* Missing `Income` values are handled using the median.
* Duplicate records are checked and removed where necessary.
* Additional features such as **Age**, **Customer Tenure**, **Total Spending**, and **Total Children** are created.
* Some categorical variables are simplified for analysis.
* Identifier, date/year, and redundant variables are removed.
* Categorical features are converted using one-hot encoding.
* Numerical features are standardized using `StandardScaler`.

## Dimensionality Reduction

**Principal Component Analysis (PCA)** is used to reduce the transformed feature space to two principal components.

This allows the customer data to be represented in a lower-dimensional space for clustering analysis and visualization.

## Clustering Methods

### K-Means Clustering

K-Means clustering is applied to divide customers into groups based on similarities in their transformed feature representations.

The number of clusters is evaluated using:

* Elbow Method / WCSS
* Silhouette Score

### Agglomerative Clustering

Agglomerative Clustering is also applied to identify hierarchical customer segments using the selected cluster count.

The resulting clusters are analyzed using customer characteristics such as income, spending behavior, household information, and campaign response.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Project Structure

```text
SmartCart/
│
├── Smart_Cart.ipynb
├── smartcart_customers.csv
└── README.md
```

## Key Learning Outcomes

This project demonstrates practical implementation of:

* Unsupervised Machine Learning
* Customer Segmentation
* Feature Engineering
* Data Preprocessing
* Feature Encoding
* Feature Scaling
* PCA
* K-Means Clustering
* Agglomerative Clustering
* Cluster Evaluation
* Exploratory Data Analysis

## Repository

This repository contains the complete Jupyter Notebook implementation and the dataset used for the SmartCart customer segmentation project.
