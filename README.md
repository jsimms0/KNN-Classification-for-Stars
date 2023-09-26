# KNN Classification for Stars
This project leverages various star characteristics to accurately classify and understand different star types using visualization techniques and machine learning algorithms, with a primary focus on the K-Nearest Neighbors (KNN) classifier.

## Skills Used:
This project uses the following data analysis skills: data understanding and exploration, data visualization, data preprocessing, handling categorical data, feature scaling, modeling and machine learning (K-Nearest Neighbors (KNN) Algorithm- a supervised machine learning classification algorithm), hyperparameter tuning, model evaluation, statistical analysis, and model interpretation.

## Project Summary:
**Goals:**
1. To understand the characteristics of stars based on various features 
2. To categorize stars into their respective types using a K-Nearest Neighbors (KNN) classifier.
3. To visualize and analyze relationships and correlations between star features.

**Data Overview:**
The dataset consists of 240 star entries, each with seven attributes: temperature (in Kelvin), luminosity (L, in L/Lo), radius (R, in R/Ro), absolute magnitude (A_M), color, spectral class, and type (Star type, categorized from 0 to 5).

## Data Visualization & Analysis:
**Data Visualization Methods:**
* Histograms: Revealed the distribution of star features and showed that features like 'Temperature' and 'A_M' had varied distributions across different star types.
* Scatter Plots: Allowed examination of relationships between variables. e.g., there seemed to be clusters in the Temperature vs. Luminosity scatter plot, hinting at different star types.
* Box and Violin Plots: Gave insights into potential outliers in the dataset and the data distribution for each feature.
* Heatmaps: Displayed correlation between variables. There were noticeable correlations between some of the features.
* Pair Plot: Offered a pairwise relationship across the entire dataframe, providing comprehensive insights.

**Data Preprocessing:**
* Handling Categorical Data: 'Color' and 'Spectral_Class' were transformed using one-hot encoding, generating new columns for each category.
* Scaling: Applied StandardScaler to standardize the features, making them suitable for modeling, especially with distance-based algorithms like KNN.

**Modeling:**
* A K-Nearest Neighbors (KNN) classifier was used. Initial testing was done with a K value of 1.
* The performance was evaluated using a confusion matrix, classification report, and accuracy. The accuracy for K=1 was ~93%.
* An error rate plot for various K values determined the optimal K value was indeed 1.

## Conclusions:
* The star dataset presents a rich variety of features that can effectively classify stars into their respective types. Visual analysis shows distinct patterns and clusters, especially when comparing features like Temperature vs. Luminosity.
* The KNN classifier, with an optimal K value of 1, achieved an accuracy of ~93%. This suggests that the features selected have a significant influence on the star 'Type', and the closest neighbour is often of the same star type.
* While the KNN model provided high accuracy, exploring other algorithms might offer even better or complementary insights. To expand this project I may delve deeper into potential outliers and see how they might impact the model's performance.
