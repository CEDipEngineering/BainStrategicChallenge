# BainStrategicChallenge

Initially as a group, we decided to divide the data into clusters before applying any form of regression, as a genreal regressor would most likely prove extremely innacurate. This division was made first into each product_type. Applying several models to it we found that the Random Forest Regressor showed the most promise. Another strategy for the division of the data that was used was to divide each city into its own separate universe, and then build a regressor for each individual product. Applying the random forest regressor model to this structured approach produced the best results we were able to achieve.

Some of the challeging problems that were found during the project were the multitude of missing values, which had to be dealt with in a few different ways, detailed in the notebooks, and the first few years of the dataset were mostly empty for the majority of the known datapoints. Another big challenge was the complete lack of numerical features, as the only numerical feature was the area, which was to be predicted. As such the other features were either one-hot-encoded or used to separate the data. Finally the years were ordinally encoded, or simply reduced to numerical entries which were then scaled. In some cases, certain products were only introduced into production very recently, as was the case with Açaí, which in many cities only had as few as 2 or 3 points, which obviously made it much more difficult to predict their trending area changes.

- The initial study into each product type can be found in the subdivisions directory.
- The latter study into individual cities and their products can be found in the 'city_clustering_v2.ipynb' notebook.
- The results can be found in the results directory.

