📌 Overview

This project implements customer segmentation on the Mall Customers dataset (200 customers) using K-Means clustering.
The goal is to group customers into distinct segments based on their annual income and spending score, enabling businesses to design targeted marketing strategies and improve resource allocation.

📊 Dataset

File used: Mall_Customers.csv

Size: 200 records

Features:

CustomerID – unique identifier

Gender

Age

Annual Income (k$)

Spending Score (1–100)

⚙️ Approach

Data Preprocessing

Selected Annual Income (k$) and Spending Score (1–100) as clustering features.

Scaled features to ensure equal weightage in clustering.

Clustering

Applied K-Means clustering (init='k-means++').

Determined optimal number of clusters using the Elbow Method (Within-Cluster Sum of Squares, WCSS).

Validated cluster quality using the Silhouette Score.

Visualization

Plotted the Elbow curve to identify the best value of k.

Visualized final clusters and centroids in 2D.

📈 Results

Optimal clusters (Elbow Method): k = 5

Silhouette Score: ~ 0.40 (moderate cluster separation)

Cluster characteristics:

Group 1: High income – High spending (Premium customers)

Group 2: High income – Low spending (Potential churners)

Group 3: Medium income – Medium spending

Group 4: Low income – High spending (Value seekers)

Group 5: Low income – Low spending (Budget customers)

🚀 Outcome

Built a segmentation model that helps businesses:

Identify high-value customers for loyalty programs.

Recognize low-engagement customers needing targeted promotions.

Improve customer relationship management (CRM) by allocating resources effectively.

🛠️ Tech Stack

Languages: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

📌 How to Run

Install dependencies:

pip install pandas numpy matplotlib seaborn scikit-learn


Open and run the notebook:

jupyter notebook Customer_Segmentation_using_K_Means_Clustering.ipynb

📌 Future Improvements

Include additional features (Age, Gender, Purchase history).

Experiment with other clustering methods (DBSCAN, Gaussian Mixture Models, Hierarchical Clustering).

Build an interactive dashboard (Streamlit / PowerBI) for real-time customer segmentation.
