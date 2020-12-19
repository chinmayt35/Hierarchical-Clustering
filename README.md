# Hierarchical-Clustering
## Overview
* Casino XYZ was looking for a new way to build a more personalized experience for its customer base. Currently the Casino leverages a one-dimensional tiering system based on Gold. Silver and Rewards tiers. These tiers are then used for planning purposes by the Casino to schedule and develop marketing campaigns. 
* However, in today's competitive environment, customers want more relevant content that suits their needs and preferences. As a result, unsupervised ML techniques were leveraged using data from the Casino’s loyalty program to identify and build seven customer personas based on a hierarchical clustering algorithm. 
* These personas would serve as an internal segmentation for the Casino that would be leveraged for more personalized targeted campaigns.

## Data overview
* The data used for the clustering algorithm included customer ID level data. 
* Features of the dataset comprised of a wide range of types from categorical to numerical ones. These included demographic data points such as gender, city and marketing consent preferences, to numerical features such as monetary KPIs, frequency metrics and marketing comp data. 
* Using feature engineering, additional features were generated to provide better behavioral indicators. For example, a lapse flag was created to identify players that churned over the course of the previous 12 months.

## Model Development
* By using a hierarchical model, categorical features did not need to undergo any numeric encoding or scaling. The only hyperparameters that were needed for the hierarchal based clustering included a defined distance metric and link function. A distance matrix needed to be defined for both numerical and categorical features, which measured how far apart two instances were from one another.
* We used the Euclidean distance metric on numeric features and the Hamming distance metric on categorical features. We then then combined both distance metrics into a custom defined function via a weighted average for use in the hierarchical model.
* The Ward linkage calculated the distance between cluster centroids, which was good for globular data and getting evenly sized clusters.

## Results
* Using pre-existing features in addition to engineered ones, the dataset was run through a hierarchical based clustering algorithm to determine similar clusters within the dataset. 
* The resulting optimal number of clusters of seven paved the way for the development of seven personas.
* These seven personas shared vast differences between one another in terms of demographic, monetary and frequency based KPIs. It also indicated the need for the Casino to move away from the tiered model and instead focus on an internal segmentation/personification of its customer base when it came to developing marketing campaigns. 
* The personas also enabled Casino Woodbine to identify their “true” high value base, customers that naturally enjoyed gambling (sure things), customers that could be ignored (lost causes) and customers that should be comped (persuadable).
