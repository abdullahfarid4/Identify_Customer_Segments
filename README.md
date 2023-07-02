# Identify_Customer_Segments
# Udacity Project

In this project, I work with real-life data provided by Bertelsmann partners AZ Direct and Arvato Finance Solution. 
The data here concerns a company that performs mail-order sales in Germany. 
Their main question of interest is to identify facets of the population that are most likely to be purchasers of their products for a mailout campaign. 
As a data scientist, I used unsupervised learning techniques to organize the general population into clusters, then used those clusters to see which of them comprise the main user base for the company. 
Prior to applying the machine learning methods, I assessed and cleaned the data in order to convert the data into a usable form.


# Step 1: Preprocessing
    I first explored and understood the data that you are working with. In this (and the next) step of the project, I worked with the general demographics data. As part of my investigation of dataset properties, I attended to a few key points:

1) How are missing or unknown values encoded in the data? Are there certain features (columns) that should be removed from the analysis because of missing data? Are there certain data points (rows) that should be treated separately from the rest?
   
2) What assumptions must be made in order to use each feature in the final analysis? Are there features that need to be re-encoded before they can be used? Are there additional features that can be dropped at this stage?
   
I created a cleaning procedure that you will apply first to the general demographic data, then later to the customers data.

# Step 2: Feature Transformation
    Now that your data is clean, I used dimensionality reduction techniques to identify relationships between variables in the dataset, resulting in the creation of a new set of variables that account for those correlations. In this stage of the project, I attended to the following points:

1) The first technique that I performed on your data is feature scaling.

2) Once I’ve scaled the features, I applied principal component analysis (PCA) to find the vectors of maximal variability. How much variability in the data does each principal component capture? Can you interpret associations between original features in your dataset based on the weights given on the strongest components? How many components will you keep as part of the dimensionality reduction process?

I used the sklearn library to create objects that implement your feature scaling and PCA dimensionality reduction decisions.

# Step 3: Clustering
    Finally, on the transformed data, I applied clustering techniques to identify groups in the general demographic data. I then applied the same clustering model to the customers dataset to see how market segments differ between the general population and the mail-order sales company. I tackled the following points in this stage:

1) Use the k-means method to cluster the demographic data into groups.
   
2) Apply the techniques and models that you fit on the demographic data to the customers data: data cleaning, feature scaling, PCA, and k-means clustering and compare the distribution of people by cluster for the customer data to that of the general population. 

   
