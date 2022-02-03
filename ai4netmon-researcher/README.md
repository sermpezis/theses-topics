# Researcher for AI4NetMon project


Do the following tasks in python. 


## Task 1: Exploratory data analysis

- Load the [AI4NetMon dataset]( https://github.com/sermpezis/ai4netmon/tree/main/data/aggregate_data ) that containts information about networks (rows; the "ASN" is id of each network) and their characteristics/features (columns)
- How many numerical and how many categorical features it has?
- How many categories each categorical feature has?
- Pick a numerical feature and plot its distribution in a CDF plot; hint: if needed you can use log-scale in some axis for better readability
- Pick a categorical feature with 3<= categories <=10 and plot its distribution in a histogram plot
- Find the pair of features with the highest correlation



## Task 2: Basic ML

- Load the [dataset](https://github.com/sermpezis/ai4netmon/tree/main/data/similarity) `ripe_ris_distance_pathlens_100k_20210701.csv`that contains a matrix with the distances between monitors (Each row/column corresponds to a monitor; monitor ids are the rows/column headers and are IPaddresses; the values of the matrix are the distances)

- Do clustering using Kmeans, with K=10 clusters. Use the distances as features, i.e., rows of the distance matrix correspond to each monitor and columns are the "features". (note: some values are NaN; it's not a problem, no need to do anything)

- Select randomly two monitors per cluster (write dows their id)

- Implement a function that for each monitor returns the 5 monitors with the largest/smallest distance (clarification: that does NOT need any ML method)

- If the number of clusters (K=10) was not given to you, how would you select a good value for K? (no need to code, you can just explain)

