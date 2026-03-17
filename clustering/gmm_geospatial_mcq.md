# Gaussian Mixture Models & Geospatial Data (MCQ)

## 📌 Overview
This document contains multiple-choice questions and explanations covering:
- Gaussian Mixture Models (GMM)
- Expectation-Maximization (EM)
- Clustering techniques
- Geospatial data with GeoPandas

---

## 🧠 Questions & Answers

### Question 1
**Which type of clustering does GMM perform?**

✅ Soft clustering  

**Explanation:**  
GMM assigns probabilities to each data point for belonging to different clusters.

---

### Question 2
**Customers belong partially to multiple segments. What does this indicate?**

✅ GMM assigns probabilities to cluster memberships  

**Explanation:**  
Each data point can belong to multiple clusters with different probabilities.

---

### Question 3
**What distribution is used in GMM?**

✅ Gaussian distribution  

**Explanation:**  
Each cluster is modeled using a normal (Gaussian) distribution.

---

### Question 4
**Can GMM handle non-spherical clusters?**

✅ Yes  

**Explanation:**  
Unlike K-Means, GMM can model clusters of different shapes.

---

### Question 5
**How are initial parameters chosen?**

✅ Randomly  

**Explanation:**  
GMM starts with random initial values and improves them using EM.

---

### Question 6
**Purpose of EM algorithm?**

✅ Update Gaussian parameters to best fit the data  

**Explanation:**  
EM iteratively improves model parameters.

---

### Question 7
**Covariance matrix representation in high dimensions?**

✅ Full matrix  

**Explanation:**  
Captures relationships between all features.

---

### Question 8
**How to handle dominant clusters?**

✅ Use weight values  

**Explanation:**  
Weights balance the influence of clusters.

---

### Question 9
**Purpose of Expectation step?**

✅ Calculate probabilities of cluster membership  

---

### Question 10
**Probabilities: 0.5, 0.3, 0.2 → Assign to?**

✅ Cluster 1  

**Explanation:**  
Choose the highest probability for hard assignment.

---

### Question 11
**Python library for geospatial data?**

✅ GeoPandas  

---

### Question 12
**GeoPandas included in Pandas?**

❌ False  
✅ True (Correct Answer: True — must be installed separately)

---

### Question 13
**What is stored in 'geometry' column?**

✅ Points, lines, polygons  

---

### Question 14
**Method to read geospatial files?**

✅ read_file  

---

### Question 15
**Can hierarchical clustering group regions?**

✅ True  

---

### Question 16
**How to show extra dimension in 2D plot?**

✅ Vary point size  

---

### Question 17
**Purpose of StandardScaler?**

✅ Normalize data (mean = 0, std = 1)  

---

### Question 18
**Ward linkage minimizes?**

✅ Within-cluster variance  

---

### Question 19
**GeoPandas supports multiple layers?**

✅ True  

---

### Question 20
**Best way to visualize 3 variables in 2D?**

✅ Scatter plot with size and color variation  

---

## 📊 Key Takeaways

- GMM uses **soft clustering**
- EM algorithm is used for **parameter optimization**
- GMM handles **non-spherical clusters**
- GeoPandas is essential for **geospatial analysis**
- Visualization can represent multiple dimensions using **size and color**

---

## 🚀 Final Thoughts
Understanding GMM and geospatial data is crucial for real-world applications like:
- Market segmentation
- Urban planning
- Customer analytics
