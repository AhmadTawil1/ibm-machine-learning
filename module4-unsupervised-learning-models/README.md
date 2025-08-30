# 📘 Module 4 – Unsupervised Learning: Clustering & Dimension Reduction  

This module explores **unsupervised learning techniques** where the goal is to discover hidden structure in unlabeled data. It covers clustering algorithms, density-based methods, and dimension reduction techniques.  

---

## 🔑 Topics Covered  
- **Clustering Strategies**  
  - Partition-based (K-Means)  
  - Density-based (DBSCAN, HDBSCAN)  
  - Hierarchical (Agglomerative & Divisive)  

- **Dimension Reduction**  
  - PCA (Principal Component Analysis)  
  - Nonlinear methods: t-SNE & UMAP  

- **Feature Engineering via Clustering**  
  - Using clustering to detect redundant features  
  - Combining feature selection & reduction  

---

## 🧪 Labs Completed  

### 1. K-Means Customer Segmentation  
- Generated synthetic data with `make_blobs`.  
- Applied K-Means clustering (`init="k-means++"`, 4 clusters).  
- Visualized clusters and centroids.  
- Tested different `k` values → observed merging/splitting.  
- **Key insight:** Choosing `k` is critical; K-Means assumes spherical clusters.  

---

### 2. Comparing DBSCAN vs HDBSCAN  
- Applied DBSCAN and HDBSCAN to Canadian museum geospatial data.  
- Visualized clusters on a map with GeoPandas.  
- DBSCAN worked for arbitrary shapes but struggled with varying densities.  
- HDBSCAN adapted better, produced cleaner clusters, no need for ε.  
- **Key insight:** HDBSCAN is more robust for real-world noisy datasets.  

---

### 3. PCA Lab  
- Applied PCA on 2D correlated and higher-dimensional datasets.  
- Projected onto principal components.  
- Analyzed **explained variance ratio**.  
- **Key insight:** PCA reduces dimensions while preserving variance → useful for denoising and preprocessing.  

---

### 4. t-SNE vs UMAP Lab  
- Compared PCA, t-SNE, and UMAP on synthetic 3D blob data.  
- **PCA:** worked well on linearly separable data.  
- **t-SNE:** preserved local clusters but slower and sensitive to hyperparameters.  
- **UMAP:** balanced local + global structure, scalable and clean clusters.  
- **Key insight:** PCA is best for compression, while t-SNE/UMAP are best for visualization of nonlinear embeddings.  

---

## 📈 Key Learnings  
- **Clustering** groups unlabeled data → useful for segmentation, anomaly detection, and feature engineering.  
- **Density-based methods** (DBSCAN/HDBSCAN) outperform K-Means on noisy, irregular data.  
- **Dimension reduction** (PCA, t-SNE, UMAP) simplifies high-dimensional datasets, improves visualization, and supports clustering.  
- **Feature engineering** with clustering helps identify redundant features, improving efficiency and model quality.  

---

## 🚀 Applications to Projects  
- **Trackr:**  
  - K-Means for discovering study behavior groups.  
  - PCA to reduce redundant behavioral features.  
  - UMAP to visualize study patterns.  
- **NeuroFocus:**  
  - PCA to compress EEG signals.  
  - HDBSCAN for adaptive clustering of focus states.  
  - t-SNE to visualize brainwave embeddings in 2D clusters.  

---

## 🧠 Reflection  
- ✅ Comfortable with clustering methods and their assumptions.  
- ✅ Learned to preprocess with PCA before nonlinear reduction.  
- ❓ Still curious about scalability of t-SNE vs UMAP on very large datasets.  
- 💡 Idea: Apply UMAP to NeuroFocus EEG data for visualization and HDBSCAN for stable state clustering.  

---

📌 **Next Module → Module 5: Recommender Systems**  
