# Tik-Tok Content Moderation: Classifying Video Claim Status for Tik-Tok
Using Categorical Gradient Boosting Machine Learning

### Problem Statement
There is a backlog of user reports for classifying Tik-Tok video as “Claims” or “Opinions”, posing a challenge to timely content moderation and accurate content recommendation on users feed. 
### Solution
We need to create a classification algorithm to solve this problem.

### Feature Engineering
We are using engagement
metrics such as **video views,
comments, shares, downloads
and transcription length** to
determine the video’s claim
status. The transcription
length is defined as the
number of characters is the
transcript of the video.

![Feature Engineering](https://github.com/hamza-safwan/Machine-Learning/blob/main/TikTok%20Content%20Moderation/feature_importance.jpg)

### Model Development
The model development involved training a Categorical Gradient Boosting Machine Learning model, specifically XGBoost using above feature engineering.
### Model Accuracy
The model developed is
extremely accurate, while
avoiding false classification of
the video claim status. It was
also constructed such that it
handles randomness in data
and bias.

![Model Accuracy](https://github.com/hamza-safwan/Machine-Learning/blob/main/TikTok%20Content%20Moderation/confusion_matrix.jpg)
### Key Insights
- The model indicate that the features with most predictive power towards video
claim status are the video view count, transcription length and the like count. This
could suggest that claim status is also related to video’s content.
 - The metrics used to evaluate the model indicate that it does not predict false
positives nor false negatives with high frequency, we see that out of all 2900+ test
samples only 9 were classified incorrectly.

### Summary
- Developed a machine learning model that classifies TikTok videos as "claims" or
"opinions" with **more than 95% accuracy**, leveraging feature engineering and fine-tuning to
optimize predictive power.
- Engineered features through selection, extraction, and transformation to prepare data for
modelling, enabling the detection of subtle patterns and relationships that drive accurate
claim/opinion classification.
- Fine-tuned the model through iterative evaluation and hyperparameter adjustment,
achieving exceptional performance and informing data-driven decisions to improve
content moderation and user experience.
