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

I do 2 important things over here - 

* missing values imputation and
* feature engineering

### Modelling:

This is where I created a train, test and validate split of the dataset.

Then I trained various models, out of the box, on the train data and compared their F1 macro score on the validation data.
Using the conclusions drawn from their, I decided on the best models and tuned the hyperparameters.

----------------

I have included the data in the [`./input/` directory](https://github.com/nityeshaga/costa_rican_poverty_prediction/tree/master/input)
and my kernel is present in the [`./notebook/` directory](https://github.com/nityeshaga/costa_rican_poverty_prediction/tree/master/notebook)
