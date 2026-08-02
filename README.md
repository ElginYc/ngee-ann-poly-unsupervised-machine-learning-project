# Ngee Ann Polytechnic Unsupervised Machine Learning Project

## Overview

A Data Analytics project that applies unsupervised machine learning techniques to a dataset containing information on 100 bank customers. Each customer is described by 20 features, including age, housing, years as a resident, car ownership, and other customer-related attributes. The project focuses on analyzing numerical data to discover hidden patterns and identify customer clusters.

- *Bank Data*

The project covers:

- Data Preprocessing
- Machine learning model development
- Model evaluation

## Data Preprocessing

The dataset was prepared before applying clustering algorithms. The preprocessing steps include:

- Identifying and handling missing values.
- Removing categorical features as the clustering models were built using numerical data only.
- Selecting relevant numerical features for customer segmentation.
- Removing the target variable since this is an unsupervised learning problem.
- Applying feature scaling and normalization to ensure numerical features are on a comparable scale.

### Dataset

- **Dataset:** 'Bank_data.csv'

## Tools & Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
  - K-Means Clustering
  - Agglomerative Clustering
  - StandardScaler
  - Normalization
  - Silhouette Score
- SciPy
  - Hierarchical Clustering
  - cdist (Distance Calculation)

## Machine Learning Models

- K-Means Clustering
- Hierarchical Clustering (Agglomerative)

## Project Files

| File                                               | Description                                                                                                                                      |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| `Unsupervised_Machine_Learning_Project.ipynb`      | Jupyter Notebook containing the complete unsupervised machine learning workflow, including clustering, and model evaluation. |
| `Unsupervised_Machine_Learning_Project_Report.pdf` | Full project report containing the methodology, analysis, results, and conclusions.                                                              |
| `Bank_Data.csv`                                    | Bank customer dataset used for clustering analysis.                                                                                              |


