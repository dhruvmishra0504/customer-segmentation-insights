# Customer Segmentation Insights

This project segments customers into meaningful groups based on their purchasing behavior, enabling data-driven marketing and customer relationship strategies.

## 📌 Project Overview
I built this project to analyze transactional retail data and identify customer segments using **RFM analysis** (Recency, Frequency, Monetary value) combined with multiple clustering algorithms.

The segmentation helps businesses:
- Identify high-value customers
- Plan targeted marketing campaigns
- Improve customer retention

## 📊 Dataset
- **Source:** [Online Retail II Dataset - UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/502/online+retail+ii)  
- Real transactions from a UK-based online retailer (2009–2011)  
- Includes invoice dates, quantities, prices, and customer IDs

## 🛠️ Features
- **Data preprocessing**: Cleaning nulls, removing cancellations, feature engineering
- **RFM analysis**: Recency, Frequency, Monetary value calculation
- **Clustering models**:
  - KMeans
  - DBSCAN (added for density-based clustering)
  - Agglomerative Clustering
- **Dimensionality reduction**: PCA for 2D visualization
- **Evaluation**: Silhouette score, Davies–Bouldin index
- **Database integration**: Export cluster profiles to SQLite
- **Dashboard**: Interactive exploration using Streamlit

## 📈 Workflow
1. **Data Cleaning & RFM Creation**  
   Transform raw sales data into RFM features.
2. **Scaling & Dimensionality Reduction**  
   Apply StandardScaler and PCA.
3. **Clustering**  
   Train models (KMeans, DBSCAN, Agglomerative) and evaluate.
4. **Cluster Profiling**  
   Analyze customer groups and export results.
5. **Visualization**  
   Build a dashboard for business stakeholders.

## 🚀 How to Run
```bash
# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook notebooks/CustomerSegmentation.ipynb

# Launch dashboard
streamlit run src/dashboard.py
