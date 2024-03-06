In this module challenge I used the StandardScaler() module from scikit-learn to normalize the data from the CSV file.
A new dataframe with the scaled data  was then formed with the "coin_id" as the index from the original dataframe as the new index.
I then referenced that dataframe by showing the head.

I then used to elbow method to find the best value for k.
I created a list with the k values of 1 to 11. I made an empty list to store those inertia values.
I then used a for loop to compute each inertia with the possible value of k.
A dictionary with the data was then used to plot the elbow curve. I plotted a line chart with all interia values computed with the different values of k.
I used this chart to identify the optimal value for k and answer my first question in this challenge..

For the second portion I created a scatter plot using clustered cryptocurrencies with K-Means. 
In order to do this I initialized k-means and fit it using the original scaled dataframe with the best value for k.
I created a copy of the original data and added a new column with the predicted clusers.
For the scatter plot I used PC1 as the x-axis and PC2 for the y-axis. I then addthe the 'coin_id' column in the hover_cols parameter to identify the cryptocurrency
represented by each data pont.

In the next portion I used the same DataFrame to perform a PCA and reduce the features to 3 components.
I then created a new DataFrame with the PCA data and again set the 'coin_id' index from that original dataframe as the new index as well.
I displayed the first 5 rows of the PCA DataFrame.



The next portion I used to new elbow method on the PCA data to find the best value for k in this dataframe.
I created a list of the k values of 1 to 11 and fit the k-means model using the PCA data.  I made an empty list to store those inertia values.
I then used a for loop to compute each inertia with the possible value of k.
A dictionary with the data was then used to plot the elbow curve. I plotted a line chart with all interia values to visualized the different values of k and see the optimal value for it.
I used this chart to identify the optimal value for k using the PCA Data and how it differed found using the original data.


For the last portion, I predicted the clusters to group the cryptocurrencies using the PCA Data.
I used the k-means model again to find the best value for k and fit it using the PCA data.
I make a new column with the predicted clusters and stored it in the new dataframe.
I used another scatter plot using hvplot. I set the x-axis as the price change percentage at 24 hours. and the y-axis  as the price change percentage of 7 days.
I again added the 'coin_id' to the hover_cols parameter to identify each data point.

Altogether the new dataframes did not change the outcome of the best value for k from the original dataframes.








