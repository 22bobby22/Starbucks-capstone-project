# Starbucks Capstone Project

## Project Overview

This dataset contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some customers might not receive any offer during certain weeks.

There is transactional data showing customer purchases made on the app including the timestamp of purchase and the amount of money spent on a purchase. This transactional data also has a record for each offer that a user receives as well as a record for when a customer actually views the offer. There are also records for when a user completes an offer.

My task is to combine transaction, demographic and offer data to build a model that is able to predict whether a customer is going to respond to an offer or not. This dataset is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.

With all this taken into account I will follow these steps to build a model with a reasonable accuracy:

  1. Explore the datasets to gain a general understanding of the data.
  2. Clean the datasets to remove any unnecessary information and for them to be fit as training data for the model.
  3. Combine the clean datasets for the model.
  4. Build and compare different models with different classifiers to look for the one that works the best in this case.

## File Descriptions

Starbucks_Capstone_notebook.ipynb: Jupyter Notebook where all the code and details are present. Code outputs are also present so you shouldn't need to run any code cell.

This project is basically all contained in the Jupyter Notebook, besides that there is also a blog post in this link that summarizes the findings detailed in the notebook: [medium blog post](https://medium.com/@crack461/starbucks-capstone-project-538116016700?source=friends_link&sk=a83922e49a9ffdb6798196e9f6fc1869)

## Dependencies

Besides Jupyter Notebook and Python 3, you can see all the imports needed in the notebook, most important being:
  - Pandas
  - Numpy
  - Matplotlib
  - Sklearn.

## Conclusion

Everything is explained and more detailed in the notebook but to briefly summarize, I created a machine learning model able to predict wheter a customer is going to respond to an offer with an accuracy of 77%, which is not bad at all. This model uses Random Forest Classifier and the following parameters:
  - max_depth: 8
  - min_samples_leaf: 1
  - min_samples_split: 2
  - n_estimators: 10
