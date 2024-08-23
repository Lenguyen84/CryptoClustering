CRYPTOCURRENCY CLUSTERING CHALLENGE

Overview and Purpose:
This project aims to utilize Python and unsupervised learning to determine whether cryptocurrencies are influenced by 24-hour or 7-day price fluctuations. Initially, the original data from a .csv file was employed to determine the optimal k value, which was then visualized using an Elbow Curve, and clusters were plotted on Scatter Plots using K-Means. Subsequently, Principal Component Analysis (PCA) was applied to refine the clusters, followed by identifying the best k value (again visualized on an Elbow Curve) and plotting clusters on Scatter Plots using K-Means for the transformed data. Finally, the visualizations from the first and second steps were compared

Description:
The dataset contains information on various cryptocurrencies, including multiple values representing percentage changes in price over different time periods

Data Cleaning:
No rows needed to be dropped from the dataset due to missing or incomplete data. The data was normalized using the StandardScaler module, resulting in a modified DataFrame named 'market_data_scaled.' A Principal Component Analysis (PCA) model was subsequently applied later in the exercise

Data Visualization Techniques:
Two types of visualizations were generated for this exericse.
(a) Line graphs:

(1) all cryptocurrencies and their percent change values-
https://github.com/Lenguyen84/CryptoClustering/blob/main/output/line.lot.png

(2) Elbow Curves
https://github.com/Lenguyen84/CryptoClustering/blob/main/output/Original_elbow_plot.png
https://github.com/Lenguyen84/CryptoClustering/blob/main/output/pca_elbow_plot.png
https://github.com/Lenguyen84/CryptoClustering/blob/main/output/composite_line_plot.png

(b) Scatter plots :
https://github.com/Lenguyen84/CryptoClustering/blob/main/output/PCA_scatter_plot.png

https://github.com/Lenguyen84/CryptoClustering/blob/main/output/market_data_scatter_plot.png

https://github.com/Lenguyen84/CryptoClustering/blob/main/output/composite_clusters_plot.png

Results and Analysis:
This exercise provides answers to the following questions:
	•  After scaling the original dataset, what is the optimal value for k, as visualized using the Elbow Curve?
		○ The optimal value for k appears to be 4.
	• After optimizing the clusters with PCA, what is the total explained variance of the three principal components?
		○ The total explained variance is approximately 89
	• What is the best value for k when using the PCA-transformed data?
			§ The best value for k is 4.
	• Does this differ from the best k value found using the original data?
			§ No, both analyses suggest k = 4.
	•  What is the impact of using fewer features for clustering with K-Means after visually analyzing the cluster results?
		○ Using fewer features for clustering results in a more distinct and tighter grouping of points near the origin (0, 0) on the plot. However, some points still plot at a distance and should be considered as separate clusters. Setting k to 4 appears to be a justified choice based on this Cluster Comparison.
  
Code Assistance:
	• The Python code is located in the main folder
	• The dataset can be found in the Resources folder as "crypto_market_data.csv
 	• Xpert Learning Assistant tool









	• The dataset can be found in the Resources folder as "crypto_market_data.csv.
