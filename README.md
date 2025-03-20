# Crypto Clustering Analysis

This project focuses on clustering cryptocurrencies based on their market data using **K-means clustering** and **Principal Component Analysis (PCA)**. The goal is to identify patterns and group cryptocurrencies based on their price change percentages over 24 hours and 7 days.

---

## Project Overview

The project involves the following steps:
1. **Data Preparation**: Load and preprocess the cryptocurrency market data.
2. **K-means Clustering**: Use the elbow method to determine the optimal number of clusters (`k`) and perform clustering on the scaled data.
3. **PCA Optimization**: Reduce the dimensionality of the data using PCA and repeat the clustering process.
4. **Visualization**: Create scatter plots to visualize the clusters.

The dataset used is `crypto_market_data.csv`, which contains price change percentages for various cryptocurrencies.

---

## Technologies Used

- **Python**
- **Jupyter Notebook**
- **Libraries**:
  - `pandas` for data manipulation
  - `scikit-learn` for scaling, K-means clustering, and PCA
  - `hvPlot` for interactive visualizations
  - `matplotlib` for plotting

---

## Usage

1. **Data Preparation**:
   - Load the `crypto_market_data.csv` file into a DataFrame.
   - Normalize the data using `StandardScaler`.

2. **K-means Clustering**:
   - Use the elbow method to find the optimal value of `k`.
   - Perform clustering and visualize the results using scatter plots.

3. **PCA Optimization**:
   - Reduce the data to three principal components.
   - Repeat the clustering process and compare the results.

4. **Visualization**:
   - Use `hvPlot` to create interactive scatter plots for both the original and PCA-transformed data.

---

## Results

### Key Findings:
- **Optimal k-value**: The best value for `k` was determined using the elbow method for both the original and PCA-transformed data.
- **PCA Impact**: Using PCA reduced the dimensionality of the data while retaining most of the variance, leading to more efficient clustering.
- **Clusters**: Cryptocurrencies were grouped into distinct clusters based on their price change patterns.

### Visualizations:
- Scatter plots showing clusters for:
  - Original scaled data (`price_change_percentage_24h` vs `price_change_percentage_7d`).
  - PCA-transformed data (`PCA1` vs `PCA2`).

---
