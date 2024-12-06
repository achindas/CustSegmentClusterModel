# Online Retail Customer Segmentation - K-Means and Hierarchical Clustering Solution

## Table of Contents
* [Clustering Overview](#clustering-overview)
* [Problem Statement](#problem-statement)
* [Technologies Used](#technologies-used)
* [Approach for Modeling](#approach-for-modeling)
* [Clustering Outcome](#clustering-outcome)
* [Conclusion](#conclusion)
* [Acknowledgements](#acknowledgements)

## Clustering Overview

Clustering is an **unsupervised machine learning technique** used to group similar data points into clusters based on their inherent characteristics. It helps uncover hidden patterns and relationships in the data without relying on predefined labels. Clustering models are widely used in various domains, such as customer segmentation, document clustering, and image processing. Two commonly used clustering algorithms are **K-Means** and **Hierarchical** Clustering.

### K-Means Clustering

K-Means is a **centroid-based** clustering algorithm that partitions the data into a predefined number of clusters (k). It works iteratively to **minimize the within-cluster sum of squares (WCSS)** by assigning each data point to the nearest cluster centroid and updating the centroids based on the mean of the assigned points. K-Means is computationally efficient, works well with large datasets, and is best suited for spherical-shaped clusters. However, it requires the number of clusters (k) to be specified beforehand and is sensitive to the initial placement of centroids.

### Hierarchical Clustering

Hierarchical Clustering builds a **tree-like structure (dendrogram)** to represent data points and their hierarchical relationships. It operates in two modes:

1. **Agglomerative Clustering** (bottom-up): Each data point starts as its own cluster, and clusters are successively merged based on similarity until a single cluster or desired number of clusters is achieved.

2. **Divisive Clustering** (top-down): The entire dataset starts as one cluster and is recursively split into smaller clusters.

Hierarchical Clustering does not require specifying the number of clusters in advance and provides a visual representation (dendrogram) to analyze cluster relationships. However, it is computationally expensive for large datasets compared to K-Means.

Both algorithms have their unique strengths and are valuable tools for uncovering meaningful insights and patterns in unlabeled data.


## Problem Statement

A UK-based online retail company aims to enhance its marketing strategy by targeting customers with **personalized and relevant offers**. To achieve this, the company seeks to segment its customers based on their transactional behavior. By analyzing approximately one year of transaction data, key metrics such as `Recency` (time since the last purchase), `Frequency` (number of purchases), and `Monetary` value (total spend) were derived to represent customer behavior. 

The goal is to segment customers into distinct categories—such as high-value, medium-value, and low-value segments—based on these metrics. This segmentation will enable the company to identify its most valuable customers, optimize marketing campaigns, and improve customer engagement and retention. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

The problem involves exploring and applying clustering techniques, specifically **K-Means and Hierarchical clustering**, to achieve meaningful and actionable customer segmentation.

## Technologies Used

Python Jypyter Notebook in local PC environment has been used for the exercise. Apart from ususal Python libraries like  Numpy and Pandas, there are machine Learning specific libraries used to prepare, analyse, build model and visualise data. The following model specific libraries have been used in the case study:

- scipy
- sklearn


## Approach for Modeling

The following steps are followed to do the segmentation of online retail customers:

1. Read and Visualise the Data
2. Clean the Data
3. Transform the Data for Modelling
4. Create K-Means Model
5. Create Hierarchical Clustering Model
6. Conclusion

Some distinguishing processes in this approach include,

- Creating new features like `Recency, Frequency and Monetary` Values (RFM) from given data to feed into the models

- Visualising the Hierarchical model outcome using `Dendogram`

- Determining the optimum number of clusters by performing `Elbow-Analysis and Silhouette Scoring`


## Clustering Outcome

The clustering exercise has successfully provided valuable insights into customer segmentation for the online retail company. By leveraging both K-Means and Hierarchical clustering models, distinct customer groups with varying spending behaviors were identified. Notably, Cluster-3 customers were recognized as **high-value customers**, exhibiting significantly higher spending, greater frequency, and recent activity. These insights empower the retail company to design targeted marketing strategies, such as extending loyalty benefits to retain high-value customers and offering enticing promotions to encourage increased engagement from **low-value customers** in Cluster-1. 

This data-driven approach enhances decision-making and contributes to improved customer retention and revenue growth.


## Conclusion

Clustering models, in general, have proven to be highly effective in **segmentation exercises** across various industries. Whether it is customer segmentation in retail and banking, market segmentation in FMCG, or identifying patient groups in healthcare, clustering enables businesses to better understand their data and make informed, targeted decisions. By identifying patterns and **natural groupings within the data**, clustering provides a robust foundation for creating personalized strategies that improve customer satisfaction, operational efficiency, and overall business outcomes.


## Acknowledgements

This case study has been developed as part of Post Graduate Diploma Program on Machine Learning and AI, offered jointly by Indian Institute of Information Technology, Bangalore (IIIT-B) and upGrad.