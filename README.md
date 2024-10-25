## Gene-Phenotype Causality Analysis

### Overview

This project aims to determine if gene and phenotype embeddings can indicate causality between them. Using a dataset with phenotype descriptions, corresponding genes, and a causal flag, we explored whether embeddings of these phenotypes and genes provide any signal for gene causality.

### Problem Statement

The goal is to conduct exploratory analysis to understand if the embeddings might indicate gene causality. We aimed to evaluate relationships between phenotypes and their associated genes (both causal and non-causal) using clustering techniques to identify potential patterns.

### Approach

#### 1. Data Preprocessing

Started with a dataset comprising phenotype descriptions and corresponding genes, along with a causal gene flag.

Extracted phenotype and gene embeddings from existing pre-trained models.

Converted embeddings from string representation to numeric format for further analysis.

Combined phenotype and gene embeddings to facilitate joint analysis.

#### 2. Dimensionality Reduction

Applied PCA (Principal Component Analysis) and t-SNE (t-distributed Stochastic Neighbor Embedding) for dimensionality reduction.

Reduced the dimensions to 2 for visualization purposes, allowing us to effectively visualize and interpret the clusters.

#### 3. Visualization

Visualized the distribution of causal vs. non-causal genes using count plots.

Generated pair plots and heatmaps to understand the correlation between different embedding dimensions.

Used PCA and t-SNE plots to observe clustering patterns for both gene and phenotype embeddings.

#### 4. Clustering

Applied KMeans and DBSCAN clustering to the combined gene-phenotype embeddings to assess potential groupings.

Conducted clustering with and without scaling the data to evaluate the effect on clustering outcomes.

#### Key Findings

Clustering of combined phenotype-gene embeddings revealed differences between causal and non-causal genes.

PCA and t-SNE visualizations helped identify potential separations among embeddings, though the distinction was not entirely clear.

DBSCAN clustering showed different clustering behavior compared to KMeans, especially with scaling, indicating different grouping characteristics.

Next Steps

Further evaluate clustering performance using metrics such as silhouette score or Davies-Bouldin index to assess clustering quality.

Apply advanced clustering methods or graph-based approaches to analyze relationships between phenotype and gene embeddings more effectively.

