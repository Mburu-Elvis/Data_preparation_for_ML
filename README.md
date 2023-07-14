# Data_preparation_for_ML

understanding the problem
framing the problem
selecting a performance measure
checking the assumptions
getting the data


## 1. Data Cleaning

### Missing data

options:

- droping duplicates
- dropping empty values
- imputation

## Random sampling

A random sample is obtained by randomly selecting observations from the entire dataset without considering any specific characteristics/groups

- Useful in creating a sample without any bias

- It may not ensure proportional represantation of subgroups or important characteristics of the data

## stratified sampling

It involves dividing datasets into distinct groups/strata based on certain characteristics/variables

Observations are then randomly sampled from each stratum, ensuring that each group is represented in the sample

- It's useful when there are significant differences/imbalances within the population
- It requires prior knowledge of the stratification variables and assumes that the groups within each stratum are homogeneous

the population is divided into homogeneous subgroups called strata,
and the right number of instances is sampled from each stratum to guarantee that the
test set is representative of the overall population. If they used purely random sam‐
pling, there would be about 12% chance of sampling a skewed test set with either less
than 49% female or more than 54% female. Either way, the survey results would be
significantly biased

## Class Imbalance

It occurs when the classes in the target variable are not represented equally in the dataset.
This leads to the ML model being biased to favour the most represented class.

Techniques of handling class imbalance:-

- oversampling
- undersampling

### a. Oversampling

involves increasing the number of instances in the minority class to match the number of instances in the majority class

Can be achieved by:

- duplicating existing instances from the minority class / generating synthetic examples using (SMOTE)
- may potentially lead to overfitting

### b. Undersampling

Involves reducing the number of instances in the majority class to match the number of instances in the minority class

It helps balance the class distribution and reduce the dominance of the majority class


## Bias

Refers to the error introduced by aapproximating a real world problem with a simplifying the model

A model with high bias makes strong assumptions about the underlying data

High bias leads to overfitting

High bias models:

- linear models - cannot capture non-linear relationships

## Variance

Refers to the amount by which the model's prediction varies for the different training sets

High variance model is higly sensitive to training data and tends to overfit

Example of high variance models:

- decision trees with deep branches


### Bias-Variance Tradeoff

The bias-variance tradeoff is the balance between the model's ability to capture the underlying patterns (low bias) and its ability to generalize well to unseen data (low variance).