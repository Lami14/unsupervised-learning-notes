# Principal Component Analysis (PCA)

## 📌 Overview
Principal Component Analysis (PCA) is a dimensionality reduction technique used to reduce the number of features in a dataset while preserving as much variance as possible.

---

## 🧠 Key Concepts

### 1. Dimensionality Reduction
PCA transforms high-dimensional data into a lower-dimensional form.

### 2. Variance
PCA focuses on capturing the directions where the data varies the most.

### 3. Principal Components
- New variables created from linear combinations of original features
- Ordered by importance (variance explained)

---

## ⚙️ How PCA Works

1. Standardize the data
2. Compute the covariance matrix
3. Calculate eigenvalues and eigenvectors
4. Sort eigenvalues (highest first)
5. Select top components
6. Transform data onto new feature space

---

## 📊 Example (Python)

```python
from sklearn.decomposition import PCA
from sklearn.preprocessing import StandardScaler
import pandas as pd

# Sample data
data = pd.DataFrame({
    'x': [2.5, 0.5, 2.2, 1.9, 3.1],
    'y': [2.4, 0.7, 2.9, 2.2, 3.0]
})

# Standardize
scaler = StandardScaler()
scaled_data = scaler.fit_transform(data)

# Apply PCA
pca = PCA(n_components=1)
principal_components = pca.fit_transform(scaled_data)

print(principal_components)
