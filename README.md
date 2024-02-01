This project focuses on segmenting customers of a retail store based on their purchase history using K-means clustering algorithm. The dataset used contains information about customers including their annual income and spending score.

## Methods Used:

# Data Import and Preprocessing:
The dataset was imported using the pandas library.
Data preprocessing steps involved checking for missing values, handling categorical variables (if any), and ensuring data integrity.

# Exploratory Data Analysis (EDA):
Descriptive statistics such as mean, median, and quartiles were calculated to understand the distribution of features.
Data visualization techniques including histograms, box plots, and count plots were used to explore the distribution of variables like age, annual income, and spending score.

# Feature Selection:
For clustering, two features, namely 'Annual Income (k$)' and 'Spending Score (1-100)', were selected as they are relevant for customer segmentation based on purchase behavior.

# Determining the Optimal Number of Clusters:
The Elbow Method was employed to determine the optimal number of clusters by plotting the Within-Cluster Sum of Squares (WCSS) against the number of clusters.
The point of inflection or "elbow" in the plot signifies the optimal number of clusters. In this case, it was found to be 5.

# Model Building:
A K-means clustering model was instantiated with 5 clusters using the KMeans class from the sklearn.cluster module.
The model was trained on the selected features, 'Annual Income (k$)' and 'Spending Score (1-100)'.

# Visualization of Clusters:
The trained model was used to predict the clusters for each customer.
Scatter plots were created to visualize the clusters based on annual income and spending score.
Centroids of each cluster were also plotted to show the cluster centers.

## Results:
The K-means clustering algorithm successfully segmented the customers into 5 distinct clusters based on their purchase behavior.
Each cluster represents a different group of customers with varying levels of annual income and spending score.
