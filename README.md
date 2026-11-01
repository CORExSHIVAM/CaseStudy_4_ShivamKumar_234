# CaseStudy_4_ShivamKumar_234

# E-Commerce Customer Segmentation

## Case Study 4 – Machine Learning

### 1. Project Overview
This project focuses on segmenting e-commerce customers based on their purchasing behavior using unsupervised machine learning techniques.

The project applies **K-Means** and **DBSCAN** clustering algorithms to an RFM (Recency, Frequency, Monetary) dataset to identify meaningful customer groups and derive actionable marketing personas.

### 2. Objectives
- Analyze customer purchasing behavior using RFM analysis.
- Apply K-Means and DBSCAN clustering algorithms.
- Reduce dimensionality using PCA.
- Visualize customer segments using t-SNE.
- Compare clustering performance.
- Develop actionable marketing strategies for each customer segment.

### 3. Technologies Used
- Python
- Google Colab
- Pandas and NumPy
- Scikit-learn
- Matplotlib
- Seaborn

### 4. Dataset
The project uses an online retail transaction dataset containing customer purchase information.

Possible dataset: **Online Retail Dataset (UCI Machine Learning Repository)**

Typical features include:
- Invoice Number
- Stock Code
- Description
- Quantity
- Invoice Date
- Unit Price
- Customer ID
- Country

Dataset source: https://archive.ics.uci.edu/dataset/352/online+retail

### 5. RFM Analysis
Customer behavior will be represented using three metrics:

- **Recency (R):** Number of days since the customer's most recent purchase. Lower values indicate more recent activity.
- **Frequency (F):** Number of distinct purchase transactions made by the customer.
- **Monetary (M):** Total customer spending.

These features will be calculated using a defined analysis date and cleaned transaction records.

### 6. Methodology
1. Load the online retail dataset.
2. Clean missing values, cancellations, and invalid transactions.
3. Calculate RFM metrics for each customer.
4. Handle skewness and scale the RFM features.
5. Apply K-Means clustering.
6. Select a suitable number of clusters using the Elbow Method and Silhouette Score.
7. Apply DBSCAN clustering and tune its parameters.
8. Apply PCA for dimensionality reduction and visualization.
9. Use t-SNE to visualize customer segments.
10. Interpret cluster profiles and develop marketing personas.

### 7. Algorithms Used

**K-Means**
- Groups customers into a predefined number of clusters.
- Suitable for discovering broad customer segments.
- Requires choosing the number of clusters.

**DBSCAN**
- Groups customers based on density.
- Can identify irregularly shaped clusters and outliers.
- May classify some customers as noise.
- Its results depend on feature scaling and parameter selection.

### 8. Dimensionality Reduction
- **PCA:** Used to reduce feature dimensions and inspect customer structure while retaining as much variance as possible.
- **t-SNE:** Used to visualize customer segments in two dimensions.

Note: PCA and t-SNE visualizations are exploratory. t-SNE distances and cluster appearances should not be treated as definitive evidence of cluster quality.

### 9. Evaluation Metrics
The clustering approaches will be evaluated using:

- Silhouette Score
- Davies-Bouldin Index
- Number of clusters
- Noise/outlier percentage for DBSCAN
- Cluster sizes
- RFM cluster profiles
- Business interpretability

Silhouette scores will be calculated only where meaningful, with appropriate handling of noise and degenerate clustering results.

### 10. Customer Personas and Marketing Strategies
Potential personas will be derived from actual cluster characteristics.

| Potential Persona | Possible Marketing Strategy |
|---|---|
| Recent High-Value Customers | VIP rewards and loyalty benefits |
| Loyal Frequent Buyers | Membership programs and personalized offers |
| At-Risk Customers | Win-back campaigns |
| New or Infrequent Customers | Welcome offers and onboarding |
| Low-Engagement Customers | Relevant product recommendations |

These are illustrative personas. Actual segment names and recommendations will be based on the observed RFM profiles.

### 11. Expected Deliverables
- Cleaned dataset or reproducible preprocessing pipeline.
- RFM analysis.
- K-Means clustering results.
- DBSCAN clustering results.
- PCA visualization.
- t-SNE visualization.
- Cluster profile analysis.
- Customer personas and marketing recommendations.
- Comparison report.

### 12. Project Structure
```text
Case-Study-4-Customer-Segmentation/
├── customer_segmentation.ipynb
├── results/
│   ├── rfm_summary.csv
│   ├── cluster_profiles.csv
│   └── visualizations/
├── README.md
└── requirements.txt
```

### 13. Project Status
**Status:** Planned / In Progress

Dataset preparation, clustering, evaluation, visualization, and persona interpretation will be completed as part of the project.

### 14. Conclusion
This project aims to identify meaningful customer segments using RFM analysis and unsupervised learning. The resulting insights can help businesses improve customer retention, personalize marketing campaigns, and allocate marketing resources more effectively.

Final conclusions will be based on experimental results.

### 15. Author
**Student Project – Machine Learning Case Study**
