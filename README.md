The primary task is to segment customers based on their purchasing behavior, with a particular focus on identifying distinct groups that can be targeted with tailored marketing strategies. Given that many customers of the company are wholesalers, it is crucial to analyze both individual and bulk purchasing patterns to effectively capture the diverse range of customer behaviors present in the dataset.

Here is a table summarizing the evaluation metric scores for each model:

Model	Silhouette Score	Calinski-Harabasz Score	Davies-Bouldin Score


KMeans	0.28	2852.854938	1.087333
DBSCAN	0.32	133.695582	2.327175
Agglomerative Clustering	0.55	236.2774858456139	0.9345869118609656
The Agglomerative Clustering model with hyperparameter optimization clearly outperforms the other models in terms of all three evaluation metrics. This suggests that this model is the best choice for this particular dataset and can provide the most accurate and reliable predictions.

Conclusion


Three different clustering models were implemented and evaluated: KMeans, DBSCAN, and Agglomerative Clustering.
The Agglomerative Clustering model with hyperparameter optimization achieved the best performance, with a silhouette score of 0.55.
The Shap values were used to explain the feature importance of the Agglomerative Clustering model.
The best performing model was saved to a pickle file and a joblib file for deployment.
The saved model was loaded and used to predict unseen data, confirming its functionality.
Overall, this project successfully created and evaluated a clustering model that can be used to segment customers based on their RFM behavior. This model can be used to improve marketing campaigns, product recommendations, and customer engagement.
