# Customer Segmentation using K-Means Clustering

## 📌 Overview
This project implements **customer segmentation** on the **Mall Customers dataset (200 customers)** using **K-Means clustering**.  
The goal is to group customers into distinct segments based on their **annual income** and **spending score**, enabling businesses to design **targeted marketing strategies** and improve **resource allocation**.

---

## 📊 Dataset
- **File used:** `Mall_Customers.csv`  
- **Size:** 200 records  
- **Features:**
  - `CustomerID` – unique identifier
  - `Gender`
  - `Age`
  - `Annual Income (k$)`
  - `Spending Score (1–100)`

---

## ⚙️ Approach
1. **Data Preprocessing**
   - Selected `Annual Income (k$)` and `Spending Score (1–100)` as clustering features.
   - Scaled features to ensure equal weightage in clustering.

2. **Clustering**
   - Applied **K-Means clustering** (`init='k-means++'`).
   - Determined optimal number of clusters using the **Elbow Method** (Within-Cluster Sum of Squares, WCSS).
   - Validated cluster quality using the **Silhouette Score**.

3. **Visualization**
   - Plotted the **Elbow curve** to identify the best value of `k`.
   - Visualized final clusters and centroids in 2D.

---

## 📈 Results
- **Optimal clusters (Elbow Method):** `k = 5`  
- **Silhouette Score:** ~ **0.40** (moderate cluster separation)  

### Cluster Insights
- **Cluster 1:** High income – High spending (Premium customers)  
- **Cluster 2:** High income – Low spending (Potential churners)  
- **Cluster 3:** Medium income – Medium spending  
- **Cluster 4:** Low income – High spending (Value seekers)  
- **Cluster 5:** Low income – Low spending (Budget customers)  

---

## 🚀 Outcome
- Built a segmentation model that helps businesses:  
  - Identify **high-value customers** for loyalty programs.  
  - Recognize **low-engagement customers** needing targeted promotions.  
  - Improve **customer relationship management (CRM)** by allocating resources effectively.  

---

## 🛠️ Tech Stack
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  

---

## 📌 How to Run
1. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn

