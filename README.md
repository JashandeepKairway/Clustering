# Clustering Analysis on the Iris Dataset

## Overview
This project performs a comparative study of different clustering algorithms on the **Iris dataset** from the UCI Machine Learning Repository. The analysis involves data preprocessing, applying clustering techniques, and evaluating their performance using various metrics.

## Dataset
The **Iris dataset** consists of 150 samples of iris flowers from three species (*Setosa*, *Versicolor*, *Virginica*), with four features:
- Sepal length
- Sepal width
- Petal length
- Petal width

The dataset is loaded using `sklearn.datasets.load_iris()`.

## Preprocessing
- **Standardization**: The data is standardized using `StandardScaler()` to ensure all features have a mean of 0 and a variance of 1.
- **Principal Component Analysis (PCA)**: The dataset is reduced to **2 principal components** for visualization.

## Clustering Algorithms Used
1. **K-Means Clustering**
2. **Agglomerative Hierarchical Clustering**
3. **DBSCAN (Density-Based Spatial Clustering)**

## Evaluation Metrics
To compare clustering performance, the following metrics are used:
- **Silhouette Score**: Measures how similar an object is to its own cluster versus other clusters.
- **Davies-Bouldin Score**: Evaluates cluster compactness and separation.
- **Calinski-Harabasz Score**: Assesses the ratio of inter-cluster and intra-cluster dispersion.

## Results
A summary table of clustering evaluation scores is generated in the script.

| Algorithm       | Silhouette Score | Davies-Bouldin Score | Calinski-Harabasz Score |
|---------------|----------------|-------------------|-------------------|
| **K-Means**   | **0.4799**      | **0.7894**        | **157.3602**      |
| **Agglomerative** | **0.4467**   | **0.8035**        | **222.7192**      |
| **DBSCAN**    | **0.3565**      | **7.1241**        | **84.5103**       |

## Visualizations
The project includes the following plots:
- PCA-reduced **scatter plot** of the original dataset
- Clustering results for **K-Means**, **Agglomerative**, and **DBSCAN**
- **Color-coded scatter plots** for each algorithm
