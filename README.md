# E-commerce Product Recommendation System

## Dataset 
I have used Amazon dataset on user ratings for electronic products, this dataset doesn't have any headers.<br>
You can find the dataset here dataset(https://www.kaggle.com/datasets/vibivij/amazon-electronics-rating-datasetrecommendation/download?datasetVersionNumber=1)
<br>
In this project, I developed a robust recommendation system designed to enhance user experience in an e-commerce setting by providing personalized product recommendations. 

## Approach
The system leverages two primary methodologies:
<br>

1. Model-Based Approach (SVD):

Singular Value Decomposition (SVD) was implemented to factorize the user-item interaction matrix. This method helps to uncover latent factors that explain the observed interactions, enabling the system to make predictions about users' potential interests in various products based on patterns observed across the entire user base. SVD is particularly effective in handling sparse data, which is common in large-scale recommendation systems.

2. Hybrid Approach:

The hybrid recommendation system combines user-based and item-based collaborative filtering techniques.
User-Based Collaborative Filtering: This method identifies similarities between users based on their past interactions with products. Recommendations are made by identifying products that similar users have interacted with but the target user has not yet encountered.
Item-Based Collaborative Filtering: This method focuses on finding similarities between products themselves. It recommends products similar to those the user has already interacted with, considering the preferences of other users.
The hybrid model balances these two approaches by weighing their contributions, resulting in a more comprehensive recommendation system that takes into account both user preferences and product similarities.

## Implementation Highlights
The system was evaluated using RMSE (Root Mean Square Error) to assess the accuracy of predictions.
The model-based SVD approach provided a baseline for performance, while the hybrid method offered a more nuanced understanding of user preferences by integrating multiple perspectives.
