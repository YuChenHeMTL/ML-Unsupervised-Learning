# machine_learning_project-unsupervised-learning

### Created by: Yuchen He
## Project Goals
Perform and train unsupervised learning techniques on a wholesale data dataset. The project involves four main parts: exploratory data analysis and pre-processing, KMeans clustering, hierarchical clustering, and PCA.

## Process
### EDA + Data Preprocessing
In this step, I performed exploratory data analysis and data preprocessing to prepare the data for the unsupervised learning techniques. I performed the following steps:
1. Import the data
2. Check for null values
3. Check for outliers
4. Check for duplicates
7. Check for correlation using heatmap
5. Visualize the data and check for skewness
6. Normalize + Scale the data using MinMaxScaler

### KMeans Clustering
First, I used the elbow method to find the optimal number of clusters. I then also used silouette scoring to verify that the number of clusters chosen has the highest score. I then used the optimal number of clusters to train the KMeans model. I then visualized the clusters using a scatter plot. 

From then, I was able to deduce characteristics of each cluster from the visualizations, which are the following:
1. Cluster 0: very low region, meaning they are primarily grouped by region
2. Cluster 1: very low averages for all features, meaning they are primarily grouped by low spending
3. Cluster 2: very high channel, and also milk, grocery, detergents_paper, and delicatessen, meaning they are primarily grouped by channel and high spending in general
4. Cluster 3: very high fresh, frozen and delicatessen, meaning they are primarily grouped by high spending in these categories
### Hierarchical Clustering
In this step, I used the dendrogram method to find the optimal number of clusters, which was 4 clusters after setting the threshold to 80000, and was able to verify the number of clusters obtained from the previous step.
### PCA
In this step, I used PCA to reduce the dimensionality of the data. I then visualized the clusters using a scatter plot, which allowed me to gather evidence that the data points are actually very close to each other, despite the fact that the clusters are very distinct from each other.
## Result:
From this project, I was able to gain insights from the data sets and communicate these insights to stakeholders using appropriate visualizations and metrics to make informed decisions based on the business questions asked.

More specifically, I was able to perform unsupervised learning techniques (Centroid & Hierarchical Modelling) on a wholesale data dataset. The project involves four main parts: exploratory data analysis and pre-processing, KMeans clustering, hierarchical clustering, and PCA.

I was able to gather the following insights from the data set:
1. Through the EDA process, there were alot of data that were outliers or not applicable to the model. This was due to the fact that the data was not normalized and the data was not scaled.
2. Through the KMeans Clustering process, we were able to find the optimal number of clusters to be 4. This was done through the elbow method.
3. Through the Hierarchical Clustering process, we were able to find the optimal number of clusters to be 4. This was done through the dendrogram method.
4. Through the PCA process, we can observe that the clusters are actually quite close to each other, to the point that the different features are almost indistinguishable from each other.

Furthermore, from this data processing and analysis, we can conclude that the columns that are important for the model are:
- Fresh
- Milk
- Grocery
- Detergents_Paper

because these are the columns that have the highest variance, so it would be recommended to distinguish the clusters based on these columns.

## Challenges
- Understanding the dataset, especially the features
- Trying to optimize clusters during the KMeans Clustering process
    - Selecting the “perfect” number of clusters
- Analyzing the result of the PCA process
    - Determining the most important features
- Using advanced features of Matplotlib for plotting

## Future Goals
- Stretch: determining whether the customer is a retailer or a hotel/restaurant/cafe
- Getting a more detailed dataset
- Using more advanced unsupervised learning techniques for clustering