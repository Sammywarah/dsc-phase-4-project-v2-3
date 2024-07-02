# Showmax Personalized Recommendation System

## Overview
This project focuses on developing a movie recommendation system using collaborative filtering techniques. The system employs the K-Nearest Neighbors (KNN) algorithm with mean ratings to predict and recommend movies to users based on their past ratings.

## Business Understanding
Showmax is a subscription-based video-on-demand service that offers a wide variety of TV shows, movies, and original content for streaming over the internet. The service focuses on providing entertainment content to subscribers, emphasizing convenience, choice, and quality of the viewing experience to attract and retain customers in a competitive digital streaming market.

## Objective
The objective of this project is to develop a personalized recommendation system to enhance user engagement and satisfaction on Showmax.

## Specific Task
The specific task is to build a model that provides the top 5 movie recommendations to a user based on their ratings of other movies.

## Problem Statement
Showmax aims to provide a tailored viewing experience by recommending the top 5 movies to users based on their past ratings and viewing behaviors. The challenge is to build an effective recommendation model that accurately predicts user preferences, thereby increasing user retention and overall satisfaction with the platform.

## Project Structure

## Summary of Data Science Steps
1. **Data Preparation**: Loading and preparing the dataset for the recommendation system.
2. **Model Training**: Training the KNNWithMeans model using the Pearson similarity metric.
3. **Predictions**: Making predictions for movie ratings and recommending top N movies for users.
4. **Model Evaluation**: Evaluating the model performance using Root Mean Squared Error (RMSE).
5. **Tuned Model**: Implementing a tuned KNNBaseline model for better prediction accuracy.

## Presentation and Sources
- [Project Presentation](presentation/presentation.pdf)
- [Dataset Source](data/df_final.csv)


## Findings

### User-Based Collaborative Filtering
- **Best Model:** KNN Baseline Model

#### Interpretation of Results:
- The KNNBaseline model provided accurate recommendations with higher predicted ratings and lower RMSE, suggesting it may be more effective in recommending top movies compared to KNN with Mean and SVD.
- KNNBaseline (Before Tuning): RMSE = 0.66
- Tuned KNNBaseline: RMSE = 0.61
- Precision: 0.90
- Recall: 0.79
- F1 Score: 0.85

The KNNBaseline model successfully recommended the top 5 movies for users, considering both predicted ratings and similar movie suggestions. The model has a high accuracy F1 Score of 0.85, suggesting it is the best performing model.

### Conclusions
The tuned KNNBaseline model is more effective in predicting user preferences compared to the initial model. Improved predictive accuracy translates to more relevant and personalized movie recommendations for users.

### Recommendations
- **Use the KNNBaseline Model:** Implement the KNNBaseline model's recommendations to personalize the user experience on Showmax. This can help in engaging users by suggesting movies they are likely to enjoy based on their past ratings.
- **Generate Top 5 Recommendations:** Use the tuned model to predict ratings and recommend the top 5 movies for each user based on their past ratings and viewing behaviors.
- **Monitor and Retrain:** Regularly tune and evaluate the recommendation models with new data to ensure they adapt to changing user preferences and movie trends. This will help maintain the accuracy and relevance of recommendations.
- **Enhance User Engagement:** Focus on user feedback and engagement metrics to refine and improve the recommendation system, ensuring high user satisfaction and retention.

## Item-Based Collaborative Filtering
#### Findings:
- Achieved a mean RMSE of 0.85.
- Mean MAE: 0.65

This is a higher RMSE compared to the KNNBaseline model, suggesting lower prediction accuracy.

### Recommendations
- **Consider Hybrid Approaches:** Combine item-based and user-based methods to leverage the strengths of both, potentially improving recommendation accuracy and coverage.

### Conclusions
The item-based collaborative filtering model, while useful, demonstrated lower accuracy compared to the KNNBaseline model used in user-based collaborative filtering. Integrating it with other methods or using hybrid approaches could enhance the recommendation system’s performance on Showmax.


