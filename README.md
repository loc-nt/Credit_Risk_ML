# Credit_Risk_ML
# CHALLENGE
## Summary and Analysis

The credit risk analysis focuses on four different models: Naive Random Oversampling, SMOTE Oversampling, Cluster Centroids Undersampling, and Combination Sampling. According to the outcomes, I would recommend using the SMOTEEEN Combined technique to assess credit risk in the future.

The nature of the dataset is unbalanced classification since the number of low risks is significantly higher than the number of high risks. Applying above resampling techniques is to help solve this problem. In all models, the precision scores are 100% for low-risk, and 1% for high-risk. Meanwhile, the recall scores look better for high-risk class: the lowest is 62% for SMOTE, while the highest is 75% for Combined. This might infer that there might be many outliers that affecting the SMOTE performance. On the other hand, the recall scores for low-risk class is highest in SMOTE (69%), and lowest in Undersampling (41%).

The balanced accuracy score is consistent in most models, approximately 66% for most of the models (except the Undersampling only 55%). In other words, about 66% of the observations, in both classes, was predicted correctly in these models. 

As a banker, you would approach risks in a conservative way: you would try to predict if a customer is in a high risk status, thus allow you to have better policies to keep the risks manageable. Therefore, the recall score for high-risk class is the most important factor, since you do not want to miss too many actual high-risk cases. In contrast, the precision score might not be important at all since we are being conservative in risk assessment; thus, having high false positive (predict high, actual low) will not affect us. As a result, the Combined model, which returns the high enough score at 75%, would be a good solution for this unbalanced classification problem.
