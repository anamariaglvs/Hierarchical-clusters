# Hierarchical-clusters
This R project uses hierarchical clustering on USArrests data (US state crime statistics). It scales data, calculates Euclidean distances, and applies linkage methods like 'average'. A dendrogram helps identify natural state groupings based on crime profiles, aiding in determining the optimal number of clusters.


dist_data<-dist(USArrests)
hclust_avg <- hclust(dist_data, 'ave') #hierarchical clustering with 'average' linkage function #i compare average of clusters
plot(hclust_avg) #dendrogram
![image](https://github.com/user-attachments/assets/887456cb-f849-45c5-abfe-e628372278e2)
