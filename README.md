# Overview

In this project, we will use a credit card credit dataset from LendingClub, a peer-to-peer lending services to predict credit card risk for Fast Lending.  We will compare six supervised machine learning models to train, test, predict and then evaluate the performance and accuracy of each model to make a recommendation on which model can best predict credit card risk.

# Machine Learning Models and Results

The dataset used to train the follow models consists of 68,817 data points.  With 347 of the 68,817 being classified as "high risk" and the rest "low risk", this dataset is considererd heavily unbalanced. 

## 1. Naive Random Sampling
#### balanced accuracy score: 64.7%   |    precision: 99%    |    recall: 59%    |    f1 score: 73%

<img width="548" alt="Screen Shot 2022-07-03 at 6 04 09 PM" src="https://user-images.githubusercontent.com/100495799/177058665-7fdbfd3e-b5ee-4b57-bdf8-129ce0b69a3f.png">

## 2. SMOTE Oversampling
#### balanced accuracy score: 66.2%   |    precision: 99%    |    recall: 69%         |    f1 score: 81%

<img width="554" alt="Screen Shot 2022-07-03 at 6 08 39 PM" src="https://user-images.githubusercontent.com/100495799/177058780-d88183b6-ce13-4448-8d9e-958e35d658d1.png">


## 3. Undersampling
#### balanced accuracy score: 54.5%   |    precision: 99%    |    recall: 40%         |    f1 score: 56%

<img width="543" alt="Screen Shot 2022-07-03 at 6 10 16 PM" src="https://user-images.githubusercontent.com/100495799/177058822-7b184411-427c-4ef9-b1f3-e105289e68f6.png">


## 4. Combination (Over and Under) Sampling
#### balanced accuracy score: 64.7%   |    precision: 99%    |    recall: 57%         |    f1 score: 72%

<img width="539" alt="Screen Shot 2022-07-03 at 6 12 16 PM" src="https://user-images.githubusercontent.com/100495799/177058870-98441444-020a-4a4e-ac8a-71f43308eabc.png">


## 5. Balanced Random Forest Classifier
#### balanced accuracy score: 79.3%   |    precision: 99%    |    recall: 88%         |    f1 score: 93%

<img width="548" alt="Screen Shot 2022-07-03 at 6 13 29 PM" src="https://user-images.githubusercontent.com/100495799/177058898-54030d5d-7ce5-495c-9d98-20421e9b6467.png">


## 6. Easy Ensemble AdaBoost Classifier
#### balanced accuracy score: 93.2%   |    precision: 99%    |    recall: 94%         |    f1 score: 97%

<img width="535" alt="Screen Shot 2022-07-03 at 6 14 10 PM" src="https://user-images.githubusercontent.com/100495799/177058912-54db1cee-b5fb-4359-813f-e51228686464.png">

# Recommendation

There is a fundamental tension between precision and recall(sensitivity).  In this scenario, having a model that can predict with a high degree of precision which consumer is high lending risk vs low lending risk is critical because the impact could be catastrophic financial loss for Fast Lending if the model is inaccurate.

In summary, when comparing the performance of the six machine learning models, the Easy Ensemble AdaBoost Classifier machine learning model comes in with the highest balanced accuracy score, precision, recall and f1 scores, categorically speaking and therefore is recommended as the best model for Fast Lending to predict credit risk.
