Customer Segmentation using K-Means Clustering

Project Overview

This project focuses on customer segmentation using the K-Means clustering algorithm. The dataset used is the "Mall_Customers" dataset, which contains information about customers, such as their gender, age, annual income, and spending score. The main objective is to segment customers into different groups based on their income and spending score, which can help businesses tailor their marketing strategies to different customer segments.

Steps and Methodology

Data Preprocessing

Loaded the dataset and performed an initial inspection to understand its structure.
Checked for null values to ensure data completeness.
Replaced categorical values in the 'Gender' column with integers (0 for Male, 1 for Female).
Renamed columns for better readability:
'Annual Income (k$)' -> 'Income'
'Spending Score (1-100)' -> 'Score'
Dropped the 'CustomerID', 'Gender', and 'Age' columns to focus on the 'Income' and 'Score' columns for clustering.

Exploratory Data Analysis (EDA)

Generated pair plots to visualize the relationships between different features.
Created box plots to check for outliers in the 'Income' and 'Score' columns.

Clustering with K-Means

Applied the Elbow Method to determine the optimal number of clusters by plotting the sum of squared errors (SSE) for different numbers of clusters.
Performed hierarchical clustering using a dendrogram to visualize the hierarchical relationships between clusters.
Implemented K-Means clustering with the optimal number of clusters (5 clusters).
Predicted cluster labels and extracted the cluster centroids.

Visualization

Visualized the clusters using a scatter plot, with each cluster represented by a different color and marker.
Plotted the centroids for each cluster to highlight the center of each group.
Used a legend to label clusters and centroids for clarity.

Results

The K-Means algorithm segmented the customers into 5 distinct clusters based on their income and spending score.
The resulting clusters can be used to target specific customer groups with tailored marketing strategies.

Conclusion

This project demonstrates the application of K-Means clustering for customer segmentation. The insights gained from the clusters can be invaluable for businesses aiming to optimize their marketing efforts and improve customer satisfaction.

Files in the Repository

Mall_Customers.csv: The dataset used for clustering.

customer_segmentation.py: Python script containing the full implementation of data preprocessing, K-Means clustering, and 

visualization.

Dependencies

Python 3.x

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

Scipy

How to Run

Install the required dependencies.

Run the customer_segmentation.py script.

The script will output the visualizations and clustering results.

License

This project is licensed under the MIT License - see the LICENSE file for details.
