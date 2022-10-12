# Explain success of a bank marketing campaign

## Overview
Our goal is to compare the performance of the classifiers K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines. 
We will utilize a dataset related to marketing bank products over the telephone.
Our dataset comes from the UCI Machine Learning repository [link](https://archive.ics.uci.edu/ml/datasets/bank+marketing). 
The data is from a Portugese banking institution and is a collection of the results of multiple marketing campaigns. 
We will make use of the article accompanying the dataset [here](https://core.ac.uk/outputs/55616194) for more information on the data and features.

## Business Objective
As stated in the abstract of the article:
> The business goal is to find a model that can explain success of a contact, i.e. if the client subscribes the deposit. 
Such model can increase campaign efficiency by identifying the main characteristics that affect success, helping in a better management of the available resources 
(e.g. human effort, phone calls, time) and selection of a high quality and affordable set of potential buying customers.

## Summary of Findings
Overall, KNN is the best model for accurate predictions, achieving the highest scores among the four models with regard to different metrics:
- average precision score on the train/test set: 41.78% / 42.76%
- accuracy score on the train/test set: 90.03% / 90.28%
- weighted average precision score on the train/test set: 88% / 89%
- weighted average recall score on the train/test set: 90% / 90%
- weighted average f1 score on the train/test set: 87% / 88%

Comparing the feature importance results among the models, the most relevant features are:
- The number of employees:
  - The number of employees has a negative effect on turning people to subscribe a deposit.

- The month of contact:
  - Contacting clients in March, July, October, December, or June will make them more likely to subscribe a deposit.
  - Contacting clients in May, September, or November will make them less likely to subscribe a deposit.

- The number of days since the last contact from a previous campaign:
  - If a lot of time has passed since a client was last contacted from a previous campaign or if a client has never been previously contacted, then the client is less likely to subscribe a deposit.

- The outcome of the previous marketing campaign:
  - If a client subscribed via the previous marketing campaign or was not contacted for the previous marketing campaign, then the client is more likely to subscribe a deposit.


## Recommendations
To increase the chance that a client will subscribe a deposit:
- Schedule marketing campaigns in the months of March, July, October, December, and June.
- New clients should be contacted relatively soon.
- Contact clients relatively soon after the last contact with them from a previous campaign.
- Contact clients that subscribed via the previous marketing campaign or were not contacted for the previous marketing campaign.


## Link to Notebook

[marketing_campaign.ipynb](https://github.com/jessi88/marketing_campaign/blob/main/marketing_campaign.ipynb)
