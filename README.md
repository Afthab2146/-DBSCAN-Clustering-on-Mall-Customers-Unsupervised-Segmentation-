# -DBSCAN-Clustering-on-Mall-Customers-Unsupervised-Segmentation-
Unsupervised customer segmentation using DBSCAN. Includes k-distance graph for choosing eps, clustering Mall Customers by Age, Income, and Spending Score, and evaluating results with Silhouette Score. Visualizes clusters and noise for deeper business insights.


# 🌀 DBSCAN Clustering on Mall Customers Dataset

This project applies **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** to the popular **Mall Customers dataset**. The goal is to perform **unsupervised customer segmentation** without prior labels and discover hidden patterns in Age, Income, and Spending Score.

---

## 📂 Workflow

1. **Dataset Loading**
   - Mall Customers dataset with features:
     - Age
     - Annual Income (k$)
     - Spending Score (1-100)

2. **Preprocessing**
   - Features are standardized using `StandardScaler` to ensure fair distance-based clustering.

3. **Choosing `eps` with k-Distance Graph**
   - Use **k-nearest neighbors** to plot the **k-distance graph**.
   - The "elbow point" helps estimate a good value for `eps`.

4. **DBSCAN Clustering**
   - Run DBSCAN with chosen parameters (`eps=0.6`, `min_samples=5`).
   - Assigns each point to a cluster or labels it as noise (`-1`).

5. **Evaluation**
   - Cluster counts are displayed.
   - **Silhouette Score** is computed (if more than one cluster exists).

6. **Visualization**
   - Scatter plot of Annual Income vs Spending Score with clusters highlighted.
   - Noise points are identified distinctly.

---

## 📊 Key Insights
- DBSCAN detects **arbitrarily shaped clusters** and **noise points**.
- Unlike K-Means, it does not require specifying the number of clusters.
- The Silhouette Score gives a measure of how well-defined the clusters are.

---


