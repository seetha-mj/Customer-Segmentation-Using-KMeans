# Customer Segmentation Using K-Means Clustering

## 1. Project Overview

This project focuses on segmenting customers based on their purchasing behaviour using Machine Learning techniques.

Customer segmentation helps businesses understand different groups of customers and develop suitable marketing strategies to improve customer satisfaction and business performance.

The project uses **RFM Analysis** and the **K-Means Clustering Algorithm** to identify meaningful customer groups.

## 2. Dataset

- **Dataset:** Online Retail II
- **Source:** Kaggle
- **Period:** December 2009 – December 2011
- **Original observations:** 1,067,371 transactions

The dataset contains information about retail transactions, including invoice numbers, products, quantities, prices, invoice dates, customer IDs and countries.

## 3. Tools and Technologies

- Python
- Google Colab
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn

## 4. Methodology

The project followed these steps:

1. **Data Collection:** Imported the Online Retail II dataset into Google Colab.
2. **Data Cleaning:** Removed missing customer IDs, cancelled transactions, negative quantities and non-positive prices.
3. **Feature Engineering:** Created a Total Amount variable by multiplying quantity and price.
4. **RFM Analysis:** Calculated three important customer behaviour measures:
   - Recency: How recently a customer made a purchase.
   - Frequency: How often a customer made purchases.
   - Monetary: How much money a customer spent.
5. **Data Transformation:** Applied logarithmic transformation and StandardScaler to prepare the data for clustering.
6. **Model Selection:** Evaluated different numbers of clusters using the Silhouette Score.
7. **Clustering:** Applied the K-Means algorithm with four clusters.
8. **Evaluation and Visualisation:** Evaluated the clustering results using Silhouette Score, Davies-Bouldin Index and Calinski-Harabasz Score. PCA was used to visualise the clusters in two dimensions.

## 5. Machine Learning Algorithm

**K-Means Clustering**

K-Means is an unsupervised machine learning algorithm that groups similar observations into clusters based on their characteristics.

It was selected because the objective was to identify customer groups without having predefined customer categories.

## 6. Results and Customer Segments

Four customer segments were identified:

- **Cluster 0 – High-Value Active Customers:** Customers who purchase frequently, spend more and have purchased recently.
- **Cluster 1 – Inactive Customers:** Customers who have not purchased for a long time and generally have low purchase frequency.
- **Cluster 2 – Occasional Customers:** Customers who purchase occasionally and have moderate spending.
- **Cluster 3 – Recent Low-Spending Customers:** Customers who purchased recently but have relatively low purchase frequency and spending.

## 7. Model Evaluation

The four-cluster model produced the following evaluation results:

- Silhouette Score: 0.3649
- Davies-Bouldin Index: 0.9303
- Calinski-Harabasz Index: 5061.72

Although the two-cluster solution had a higher Silhouette Score, four clusters were selected to obtain more detailed and actionable customer segments.

## 8. Conclusion

The project demonstrates how unsupervised machine learning can be applied to customer segmentation.

By combining RFM analysis with K-Means clustering, customers were divided into four groups based on their purchasing behaviour. These findings can help businesses understand customer characteristics and develop more targeted marketing strategies.

## 9. Project Files

- `Customer_Segmentation_KMeans.ipynb` – Google Colab notebook containing the complete analysis and Python implementation.

## 10. Author

Seetha Lakshmy M J
