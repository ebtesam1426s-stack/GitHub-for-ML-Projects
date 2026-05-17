# Credit Card Customer Segmentation (K-Means Clustering)

##  Project Overview
This project focuses on segmenting credit card customers using K-Means Clustering, an unsupervised machine learning algorithm.  
The goal is to group customers based on their spending behavior in order to help businesses understand different customer types and improve marketing strategies.

---

##  Dataset
The dataset used is CC_GENERAL.csv, which contains 8,950 credit card customers and 18 behavioral features such as:
- BALANCE
- PURCHASES
- CASH_ADVANCE
- CREDIT_LIMIT
- PAYMENTS
- PURCHASES_FREQUENCY
- And more...

Each row represents a customer, and there are no target labels, making this an unsupervised learning problem.

---

##  Project Workflow

### 1. Data Preprocessing
- Removed CUST_ID column (identifier only, not useful for clustering)
- Handled missing values using mean imputation
- Checked data consistency

### 2. Exploratory Data Analysis (EDA)
- Histograms for feature distributions
- Correlation heatmap
- Scatter plots (e.g., BALANCE vs PURCHASES, CASH_ADVANCE)

### 3. Feature Scaling
- Applied StandardScaler
- Normalized all features to ensure fair distance-based clustering

### 4. Choosing Optimal K
- Used Elbow Method (Inertia)
- Used Silhouette Score
- Selected final value: K = 4

### 5. K-Means Clustering
- Trained final model using:
  - KMeans(n_clusters=4, random_state=42, n_init=10)
- Assigned cluster labels to each customer

### 6. Dimensionality Reduction (PCA)
- Reduced features to 2 components for visualization
- Plotted clusters in 2D space

---

##  Results & Insights

### Customer Segments:
- Cluster 0 – Active Spenders: Moderate balance, high purchases
- Cluster 1 – VIP Customers: Very high purchases and balances
- Cluster 2 – Cash Advance Users: High balance, low purchases
- Cluster 3 – Low Engagement Customers: Low activity overall

---

##  Business Impact
This segmentation can help companies:
- Offer cashback and rewards to active users
- Provide premium services for VIP customers
- Reduce cash advance fees for debt-heavy users
- Run reactivation campaigns for inactive customers

---

##  Technologies Used
- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn (KMeans, PCA, StandardScaler)
