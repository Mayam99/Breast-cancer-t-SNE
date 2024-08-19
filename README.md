# Breast Cancer Gene Expression Analysis using t-SNE

This project explores gene expression data from a breast cancer microarray experiment using the CuMiDa GSE45827 dataset. The dataset consists of gene expression profiles of breast cancer patients and is intended for research on identifying patterns in gene activity that correlate with cancer presence. The goal of this analysis is to apply t-SNE (t-Distributed Stochastic Neighbor Embedding) for visualizing and interpreting high-dimensional gene expression data.

Dataset Overview

The dataset includes 151 samples with 54,677 gene expression features, each representing the activity of a specific gene. The data is highly dimensional, making it suitable for dimensionality reduction and visualization techniques like t-SNE. However, the dataset does not contain pre-labeled categories (e.g., "cancerous" or "non-cancerous"). The primary focus is on identifying natural groupings or clusters within the gene expression profiles.

Key Steps in the Project:

1. Data Preprocessing:

* Handled non-numeric data by either encoding categorical variables or dropping irrelevant columns.
* Scaled the features using StandardScaler to ensure consistency in data distribution for t-SNE modeling.

2. Dimensionality Reduction (PCA):

* Applied Principal Component Analysis (PCA) to reduce the number of features from 54,677 to a more manageable set (e.g., 50 components) before running t-SNE. This step optimizes performance while preserving key variance.

3. t-SNE Visualization:

* Used t-SNE to reduce the dataset to 2 dimensions, allowing for effective visualization of potential clusters within the gene expression data.
* The t-SNE plot helps to reveal patterns or separations in the dataset that could indicate biologically relevant groupings, even without prior labeling.

Results and Insights

The t-SNE plot provides a visual representation of the high-dimensional gene expression data, highlighting potential clusters that might correspond to different biological states, subtypes, or conditions. Further analysis could involve examining the genes contributing to each cluster or applying additional clustering techniques like k-means.

Technologies Used
* Python
* scikit-learn
* pandas
* matplotlib
* seaborn
