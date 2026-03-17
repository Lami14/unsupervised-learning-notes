# Dimensionality Reduction

## 📌 Overview
Dimensionality reduction is the process of reducing the number of input features in a dataset while preserving important information.

It helps simplify models, reduce computation, and improve performance.

---

## 🧠 Why It Matters
- Reduces complexity
- Improves model performance
- Helps visualize high-dimensional data
- Removes noise and redundancy

---

## 🔑 Types of Dimensionality Reduction

### 1. Feature Selection
Selecting a subset of original features.

Examples:
- Removing highly correlated features
- Using statistical tests

---

### 2. Feature Extraction
Creating new features from existing ones.

Examples:
- Principal Component Analysis (PCA)
- t-SNE (t-Distributed Stochastic Neighbor Embedding)

---

## ⚙️ Popular Techniques

### 📊 Principal Component Analysis (PCA)
- Linear technique
- Maximizes variance
- Produces uncorrelated components

---

### 📉 t-SNE
- Non-linear technique
- Good for visualization
- Preserves local structure

---

### 📌 UMAP
- Faster than t-SNE
- Preserves both local and global structure

---

## 📊 Example (Python - PCA)

```python
from sklearn.decomposition import PCA
from sklearn.preprocessing import StandardScaler
import pandas as pd

# Sample dataset
data = pd.DataFrame({
    'A': [1, 2, 3, 4],
    'B': [2, 4, 6, 8],
    'C': [5, 7, 9, 11]
})

# Standardize
scaler = StandardScaler()
scaled_data = scaler.fit_transform(data)

# Apply PCA
pca = PCA(n_components=2)
reduced_data = pca.fit_transform(scaled_data)

print(reduced_data)
