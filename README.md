# Anomaly Detection in Yeast Dataset

This is a project for the Machine Learning 2 course at EPITA. The goal is to detect anomalies in the yeast dataset.

## Dataset

The dataset is from the UCI Machine Learning Repository and contains information about yeast cells. The dataset is available at https://archive.ics.uci.edu/ml/datasets/yeast

## Model Comparison Plan
We evaluate five multivariate models to identify the best performer for the Yeast dataset's specific topography:

* **Isolation Forest:** Tree-based isolation (excellent for high-dimensional, global anomalies).
* **Mahalanobis Distance:** Statistical distance that accounts for feature correlation (best for Gaussian-distributed clusters).
* **Local Outlier Factor (LOF):** Density-based detection (finds "local" outliers that might be normal in a global context).
* **Gaussian Mixture Model (GMM):** Probabilistic clustering (useful if the "normal" data is composed of multiple subpopulations).
* **One-Class SVM:** Geometric boundary estimation (effective for high-dimensional data with non-linear boundaries).