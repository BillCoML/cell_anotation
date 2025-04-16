# Cell Type Annotation - Project Overview

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![Status](https://img.shields.io/badge/status-Completed-brightgreen)

This repository contains code and experiments for the project **"Cell Type Annotation Using Machine Learning"**, where I classify cell types based on single-cell RNA sequencing data.

## 📂 Files

- `cell_type.ipynb`: Main notebook containing full pipeline from data preprocessing, feature engineering, to model evaluation.
- `data/train.rds`, `data/test.rds`: Raw training and testing datasets (not uploaded).

## 🔬 Project Objective

To build an accurate model that predicts cell types using gene expression levels from single-cell RNA-seq data.

## 🧪 Workflow Summary

### 1. Data Loading and EDA
- Loaded `.rds` data files using `pyreadr`
- Explored gene distributions, sparsity, and activity per cell type
- Identified highly variable genes

### 2. Feature Engineering
- Normalized and log-transformed gene expression values
- Applied PCA on top variable genes for dimensionality reduction
- Selected marker genes based on differential activity across cell types

### 3. Simulation and Cross Validation
- Set up systems for running simulation to extract metric Confidence Intervals
- Developed a reusable cross-validation function with metric tracking (precision, recall, F1-score)

### 4. Model Training and Benchmarking
- Evaluated multiple models: SVM, Random Forest, KNN, XGBoost and Neural Networks
- Computed 95% confidence intervals for each metric using t-distributions
- Developed a stacked ensemble model from top performers

## 📊 Result
The Neural Network model showed the best macro-F1 score at **98%** and balanced performance across all cell types, effectively handling extreme class imbalance.

## 📬 Contact
**Bill Co** – bill130804@gmail.com  
[LinkedIn](https://www.linkedin.com/in/bill-co-6367a3248) | [GitHub](https://github.com/BillCoML)

---

> This project was part of a university coursework on machine learning and bioinformatics.
