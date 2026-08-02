# Ngee Ann Polytechnic Unsupervised Machine Learning Project

## Overview

A Data Analytics project that applies unsupervised machine learning techniques to a dataset containing information on 100 bank customers. Each customer is described by 20 features, including age, housing, years as a resident, car ownership, and other customer-related attributes. The project focuses on analyzing numerical data to discover hidden patterns and identify customer clusters.

## Project Scope

The project covers:

- Exploratory Data Analysis (EDA) and data exploration
- Data Preprocessing
- Development of clustering models using K-Means and Hierarchical Clustering
- Model evaluation using Silhouette Score
- Customer segmentation and pattern discovery

## Data Preprocessing

The dataset was prepared before applying clustering algorithms. The preprocessing steps include:

- Identifying and handling missing values.
- Removing categorical features since the clustering models were built using numerical data only.
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


## Model Evaluation & Results

The clustering models were evaluated using the Silhouette Score to measure the quality of cluster separation. A total of 20 clustering models were tested using different feature combinations and clustering configurations.

### Best Performing Models

| Model | Algorithm | Features Used | Clusters | Linkage | Silhouette Score |
|------|-----------|---------------|----------|---------|------------------|
| Model 13 | Hierarchical Clustering | Duration in month, Credit amount | 2 | Single | 0.7822 |
| Model 15 | Hierarchical Clustering | Duration in month, Credit amount, Age in years | 2 | Single | 0.7822 |
| Model 17 | Hierarchical Clustering | Duration in month, Credit amount | 2 | Complete | 0.7467 |
| Model 11 | Hierarchical Clustering | Duration in month, Credit amount, Age in years | 2 | Average | 0.7467 |

### Final Model Selection

The selected model was:

- **Algorithm:** Hierarchical Clustering
- **Linkage:** Single
- **Features Used:** Duration in month and Credit amount
- **Number of Clusters:** 2
- **Silhouette Score:** 0.7822

The model achieved the highest Silhouette Score among all tested models. However, the clustering result showed that one cluster contained almost all observations while the second cluster contained only one observation, indicating the presence of an outlier.

Therefore, additional models were considered based on both Silhouette Score and cluster distribution.

### Final Interpretation

Models with more balanced cluster distributions were also analysed. Hierarchical Clustering using Average and Complete linkage produced more meaningful customer segmentation compared to the highest-scoring Single linkage models.

The results demonstrate that customer patterns can be identified using numerical features, particularly:
- Duration in month
- Credit amount
- Age in years

## Detailed Report

For the complete project methodology, exploratory data analysis (EDA), data preprocessing, model development, evaluation results, visualisations, and conclusions, please refer to:

`Unsupervised_Machine_Learning_Project_Report.pdf`
