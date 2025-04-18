# 102203960_ojasvi_clustering-algorithms-comparison
Comparative study of K-Means, Hierarchical, and Mean Shift clustering algorithms using different preprocessing techniques on the Iris dataset. Evaluation based on Silhouette Score, Calinski-Harabasz Index, and Davies-Bouldin Index.

# CLUSTERING ALGORITHM PERFORMANCE COMPARISON

This project is a comparative study of three clustering algorithms — **K-Means**, **Hierarchical Clustering**, and **Mean Shift** — applied on the **Iris dataset** using various preprocessing techniques. The objective is to evaluate and analyze the performance of these algorithms using different cluster sizes and metrics.

---

## 📊 Dataset
- **Name**: Iris Dataset
- **Source**: UCI Machine Learning Repository
- **Features**: Sepal and Petal lengths/widths for three iris species (setosa, versicolor, virginica).

---

## ⚙️ Algorithms Used
- **K-Means Clustering**: An iterative algorithm that partitions the data into K clusters, where each data point belongs to the cluster with the nearest mean.
- **Hierarchical Clustering (Agglomerative)**: A bottom-up approach that starts with individual points as clusters and merges them progressively.
- **Mean Shift Clustering**: A non-parametric algorithm that shifts data points towards the mode of the distribution, automatically determining the number of clusters based on bandwidth estimation.

---

## 🔄 Preprocessing Techniques
- **No Preprocessing**: Raw data with no transformations applied.
- **Standard Normalization**: Transforms features to have zero mean and unit variance.
- **PCA (Principal Component Analysis)**: Reduces the data dimensionality while retaining as much variance as possible.
- **Normalization + PCA**: Combines normalization and dimensionality reduction to improve clustering quality.

---

## 🔢 Cluster Sizes Evaluated
- **K-Means & Hierarchical**: c = 3, 4, 5
- **Mean Shift**: Cluster count is determined automatically using bandwidth estimation

---

## 📈 Evaluation Metrics
- **Silhouette Score**: Measures how similar each point is to its own cluster compared to other clusters.
- **Calinski-Harabasz Index**: A higher score indicates better-defined clusters.
- **Davies-Bouldin Index**: A lower value indicates better clustering performance.

---

## 📋 Results Summary
- **Best algorithm**: K-Means (especially with normalization)
- **Optimal cluster count**: 3 (matching true species)
- **Normalization** improved clustering performance
- **PCA** helped with dimensionality reduction but sometimes reduced score slightly

---



## ▶️ How to Run
1. Open `clustering_analysis.ipynb` in Google Colab or Jupyter Notebook.
2. Run all cells to perform clustering and generate plots.
3. Check results in the final dataframe and visual plots.


---


## ✅ Conclusion
K-Means with Normalization yielded the best clustering performance for the Iris dataset. Preprocessing significantly affects clustering quality. Mean Shift worked without needing the number of clusters but gave fewer and sometimes less accurate clusters.

---

## 🔗 References
- [Iris Dataset - UCI](https://archive.ics.uci.edu/ml/datasets/iris)
- [Scikit-Learn Documentation](https://scikit-learn.org/stable/documentation.html)
