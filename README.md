# Fundamentals of Data Science (22CSC59) - Case Studies

**Author:** Bharath Yalamanchili  
**Course:** Fundamentals of Data Science  
**Batch:** 2 (V Semester)

## Overview
This repository contains the Python implementations and Jupyter Notebooks for the Data Science course case studies. The project demonstrates the application of the end-to-end machine learning workflow—from data preprocessing and exploratory data analysis (EDA) to model training, evaluation, and business interpretation.

This submission includes solutions for **Case Study 2** (Unsupervised Learning) and **Case Study 5** (Supervised Learning).

---

## Case Study 2: Airlines Customer Segmentation (Clustering)
**Dataset:** `EastWestAirlines.xlsx`

**Objective:** 
Apply clustering algorithms to passenger flight data to discover hidden behavioral segments and identify frequent flyer archetypes to aid in targeted marketing.

**Methodology & Algorithms:**
* **Preprocessing:** Handled missing values via median imputation and scaled features using `StandardScaler`.
* **K-Means Clustering:** Utilized the Elbow Method (WCSS) to identify $K=4$ as the optimal number of clusters. 
* **Hierarchical Clustering:** Plotted a dendrogram and applied Agglomerative Clustering using Ward's linkage.
* **DBSCAN:** Applied density-based clustering to isolate standard users from extreme, high-variance outliers (noise).
* **Evaluation:** Models were evaluated using the internal Silhouette Score and visualized via 2D PCA reduction.

---

## Case Study 5: Wine Quality Assessment (Regression)
**Datasets:** `winequality-red.csv` & `winequality-white.csv`

**Objective:** 
Determine if objective physicochemical laboratory measurements can reliably predict sensory wine quality scores, and evaluate if these models can replace human taste testers.

**Methodology & Algorithms:**
* **Dual-Model Approach:** Built separate regression models for Red and White wines to preserve chemical baseline integrity and strictly adhere to the 11-attribute constraint.
* **Exploratory Data Analysis:** Computed Coefficient of Variation (CV) to find relative variability and generated correlation heatmaps to identify the strongest predictors (Alcohol and Volatile Acidity).
* **Multiple Linear Regression:** Trained models on an 80/20 train-test split.
* **Evaluation:** Models were evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and $R^2$ scores.

---

## Tech Stack
* **Language:** Python 3
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `scipy`
* **Environment:** Jupyter Notebook / Google Colab

## How to Run
1. Clone this repository to your local machine or open the `.ipynb` file in Google Colab.
2. Ensure the datasets (`EastWestAirlines.xlsx`, `winequality-red.csv`, and `winequality-white.csv`) are in the same working directory.
3. Run the notebook cells sequentially to view the data preprocessing steps, visualizations, and model outputs.
