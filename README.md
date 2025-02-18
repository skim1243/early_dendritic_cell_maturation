# README: Early Dendritic Cell Maturation Analysis

## Overview
This repository contains analysis scripts and results for studying early-stage dendritic cell maturation using transcriptomic data. The analysis includes:
- **Boxplot** for visualizing gene expression distributions
- **Heatmap** for clustering and identifying differentially expressed genes
- **Principal Component Analysis (PCA)** for dimensionality reduction and variance exploration
- **Gene Set Enrichment Analysis (GSEA)** to identify biological pathways associated with dendritic cell maturation

## Data
The dataset consists of RNA sequencing data from early-stage dendritic cells at different maturation states from https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE288378. The primary goal is to understand transcriptional changes during maturation and identify key regulatory pathways.

## Analysis Steps

### 1. Boxplot Analysis
- Visualizes the expression distribution of selected genes across different maturation stages.
- Helps identify genes with significant changes in expression levels.
- Implemented using `seaborn` and `matplotlib` in Python.

### 2. Heatmap Analysis
- Uses hierarchical clustering to group genes based on expression patterns.
- Identifies distinct gene expression signatures between immature and mature dendritic cells.
- Implemented using `seaborn.heatmap`.

### 3. Principal Component Analysis (PCA)
- Reduces dimensionality of gene expression data to capture major variance components.
- Highlights differences in gene expression between immature and mature dendritic cells.
- Identifies top genes contributing to principal components.
- Implemented using `sklearn.decomposition.PCA`.

### 4. Gene Set Enrichment Analysis (GSEA)
- Determines which biological pathways are enriched in different maturation stages.
- Uses pre-ranked gene lists based on differential expression.
- Implemented using `gseapy` for pathway enrichment analysis.

## Dependencies
Ensure the following Python libraries are installed:
```bash
pip install numpy pandas seaborn matplotlib scikit-learn gseapy
```

## Usage
1. Preprocess raw RNA-seq count data into log-transformed expression values.
2. Run individual scripts for boxplot, heatmap, PCA, and GSEA.
3. Interpret visual outputs to identify key genes and pathways involved in dendritic cell maturation.

## Results & Interpretation
- **Boxplots** highlight differentially expressed genes.
- **Heatmaps** cluster genes and samples based on expression similarity.
- **PCA plots** reveal major sources of variance in gene expression.
- **GSEA** identifies enriched pathways regulating early dendritic cell maturation.

## Contact
For questions or collaboration, please reach out via GitHub issues or email (provided upon request).

