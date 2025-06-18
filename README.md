# MSCS_634_Lab_3

The purpose of this lab is the get hands-on experience with K-Means and K-Medoids Algorithms. 

Exploratory data analysis showed the following counts for the wine target categories:
target	
- 1 -	71
- 0	- 59
- 2	- 48

First, I applied StandardScaler, which does Z Score normalization.

The first algorithm I applied was K-Means with 3 clusters. I then calculated the Silhouette Score with the following result:

- Silhouette Score: 0.2849

This score is not very high, which means the individual clusters are not well separated and compact. 

On the other hand, when I calculated the ARI, I got a very high score. ARI compares the cluster classification with the original class labels. A score of 1 means a perfect score. 

- Adjusted Rand Index (ARI): 0.8975

Afterwards, I applied the K-Medoids algorithm. Instead of finding a center of each cluster, it finds the most centered already existing point for each cluster. After calculating Silhouette and ARI scores, we can see this method was little less accurate then the K-Mean Method.

- Silhouette Score (K-Medoids): 0.2660

- Adjusted Rand Index (ARI) (K-Medoids): 0.7263

As we can see from the Scatter Plots below, K-Means algorithm provided for a little better separation and less overlap in the clusters compared to K-Medoids. The better accuracy was also reflected in the ARI and Silhouette Scores. 

![Scatter Plots](Screenshot/Scatter%20Plots.png)

