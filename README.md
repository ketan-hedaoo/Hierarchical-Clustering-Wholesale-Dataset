# 📊 Wholesale Customers Clustering (Hierarchical Clustering Project)

This project applies **Hierarchical Clustering** on the **Wholesale Customers** dataset using Python, with data preprocessing, clustering, dimensionality reduction (PCA), and visualization. The objective is to segment customers based on their purchasing behavior to derive useful insights.

---

## 🗂️ Project Structure

```
├── data/
│ └── Wholesale_customers.csv # Input dataset
├── notebooks/
│ └── hierarchical.ipynb # Main clustering script
├── outputs/
│ ├── models/
│ │ └── hierarchical.pkl # Saved clustering model
│ └── results/
│ ├── dendrogram.png # Dendrogram visualization
│ └── hierarchical_clusters.png # PCA cluster visualization
├── README.md # Project documentation
```

---

## 📌 Dataset

- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers)
- **Attributes:** Fresh, Milk, Grocery, Frozen, Detergents_Paper, Delicassen, Channel, Region
- **Target:** Not available (unsupervised learning)

In this project, we remove `Channel` and `Region` for pure clustering analysis.

---

## 🛠️ Features

- 📦 **Data Preprocessing**
  - Dropping irrelevant columns
  - Scaling with `StandardScaler`
- 🧮 **Hierarchical Clustering**
  - Dendrogram analysis
  - Agglomerative clustering (Ward method)
- 📉 **Dimensionality Reduction**
  - PCA to reduce data to 2D for visualization
- 🧾 **Model Persistence**
  - Saving and loading the clustering model using `joblib`
- 📊 **Visualizations**
  - Dendrogram
  - 2D PCA cluster scatter plot

---

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/wholesale-clustering.git
cd wholesale-clustering
