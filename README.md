# Hierarchical-clusters
This R project uses hierarchical clustering on USArrests data (US state crime statistics). It scales data, calculates Euclidean distances, and applies linkage methods like 'average'. A dendrogram helps identify natural state groupings based on crime profiles, aiding in determining the optimal number of clusters.


dist_data<-dist(USArrests)
hclust_avg <- hclust(dist_data, 'ave') #hierarchical clustering with 'average' linkage function #i compare average of clusters
plot(hclust_avg,
     hang = -1,                 # para que las etiquetas estén alineadas
     cex = 0.6,                 # tamaño de las etiquetas
     main = "Dendrogram of USArrests",
     xlab = "",                 # elimina etiqueta del eje x
     sub = "",
     ylab = "Height")   
![Rplotd](https://github.com/user-attachments/assets/eafe675c-2b41-40de-b44c-d0f41cf4ddc4)

Summary: 
-Dendrogram visualization → reveals natural groupings of states by crime patterns
-Helps identify optimal cluster count → supports insights into regional crime trends
-Scaled data + Euclidean distance → accurate measurement of state crime profile similarities 
