# Costa Rican Household Poverty Level Prediction

Analysis based on a dataset of Costa Rican household characteristics in order to improve the Proxy Means Test (or PMT)
performance.

[Here's](https://www.kaggle.com/c/costa-rican-household-poverty-prediction) the Kaggle page for this challenge.

------------------

## My Approach:

The Kernel is divided into 3 parts:

### Data Exploration:

Here I try to analyse the `Target` feature. I visualise the relationship of the `Target` variable with other features and
use the graphs to draw conclusions.

I also identified the types of features and cleaned up the inconsistency in data here.

### Preprocessing:

I do 4 important things over here - 

* missing values imputation
* generating ordinal features from dummy features
* removing redundant features
* creating new household-wide features

### Modelling:

I try Random Forest along with 2 gradient boosting machines - LightGBM and XGBoost.

I have used a 10-fold cross-validation strategy to get the CV scores for each model for comparision.

In the end, I decided on the LightGBM model and got a score of 0.429 on Kaggle's leaderboard (*currently in the top 7%*).

----------------

I have included the data in the [`./input/` directory](https://github.com/nityeshaga/costa_rican_poverty_prediction/tree/master/input)
and my kernel is present in the [`./notebook/` directory](https://github.com/nityeshaga/costa_rican_poverty_prediction/tree/master/notebook)
