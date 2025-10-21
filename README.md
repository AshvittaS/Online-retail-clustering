# 🛒 Online Retail Customer Segmentation Analysis

## 📊 Project Overview
This project performs comprehensive customer segmentation analysis on online retail data using **RFM (Recency, Frequency, Monetary)** analysis combined with multiple clustering algorithms. The analysis helps identify distinct customer groups for targeted marketing strategies.

## 🎯 Unique Features & Analysis

### 🔍 **Advanced RFM Analysis**
- **Recency**: Days since last purchase
- **Frequency**: Number of purchases made
- **Monetary**: Total money spent by customer
- Applied logarithmic transformations for better clustering performance
- Implemented outlier treatment using IQR method

### 🤖 **Multi-Algorithm Clustering Comparison**
1. **K-Means Clustering** (Silhouette Score: 0.4314)
2. **DBSCAN Clustering** (Silhouette Score: 0.4087) 
3. **Hierarchical Clustering** (Silhouette Score: 0.2702)

### 📈 **Comprehensive Data Preprocessing**
- Removed negative quantities and cancelled orders
- Handled missing CustomerID values
- Applied StandardScaler for feature normalization
- Used elbow method for optimal cluster selection

### 🎨 **Advanced Visualizations**
- 3D scatter plots for cluster visualization
- Distribution analysis with KDE plots
- Dendrogram for hierarchical clustering
- Comparative cluster analysis across algorithms

## 📊 Dataset Information
- **Total Records**: 541,909 transactions
- **Features**: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country
- **Time Period**: Online retail transactions
- **Data Quality**: Cleaned and preprocessed for analysis

## 🔧 Technical Implementation

### Data Processing Pipeline
```python
# Key preprocessing steps:
- Removed cancelled orders (InvoiceNo starting with 'C')
- Filtered positive quantities and prices
- Handled missing CustomerID values
- Created TotalPrice feature
- Applied RFM transformations
```

### Clustering Algorithms Used
- **K-Means**: Optimal k=2 clusters identified
- **DBSCAN**: eps=0.6, min_samples=3 for best performance
- **Hierarchical**: Ward linkage with 4 clusters

## 📈 Results & Insights

### Cluster Characteristics
The analysis reveals distinct customer segments:
- **High-Value Customers**: High monetary value, frequent purchases
- **At-Risk Customers**: High recency (inactive), low frequency
- **New Customers**: Recent purchases, low frequency
- **Loyal Customers**: Low recency, high frequency

### Performance Metrics
- **Best Performing**: K-Means (Silhouette Score: 0.4314)
- **Most Robust**: DBSCAN (handles noise and outliers)
- **Most Interpretable**: Hierarchical (clear cluster hierarchy)

## 🎯 Business Applications
- **Customer Retention**: Identify at-risk customers
- **Marketing Segmentation**: Target specific customer groups
- **Product Recommendations**: Based on customer behavior patterns
- **Lifetime Value Prediction**: Using RFM scores

## 📁 Files Structure
```
Online-retail-clustering/
├── OnlineRetail.csv          # Original dataset
├── task.ipynb               # Complete analysis notebook
└── README.md                # Project documentation
```

## 🚀 Key Achievements
- ✅ Comprehensive RFM analysis implementation
- ✅ Multi-algorithm clustering comparison
- ✅ Advanced data preprocessing pipeline
- ✅ 3D visualization of customer segments
- ✅ Performance evaluation across algorithms
- ✅ Business-ready customer segmentation insights

---
*This project demonstrates advanced customer segmentation techniques using machine learning clustering algorithms on real-world retail data.*
