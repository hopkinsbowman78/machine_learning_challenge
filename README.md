# sklearn-machine-learning


## Analysis Report
The purpose of this exercise was to analyze lending data and build models that may help predict a borrowers' creditworthiness. Unfortunately, we do see a significant class imbalance between healthy loans (75,036) and high-risk loans (2,500), which could negatively impact our model's performance.

After splitting the original data into training and testing datasets, the first Logistic Regression Model was created.

Then after reviewing the results of my first model, I used the resampling method with our dataset before creating the second Logistic Regression Model. Resampling will not only allow us to see how the second model will perform on data it has not been trained on, but will also help even out the class imbalance we saw before running our first model.

## Results
### Logistic Regression Model 1:

- Precision: 100% accuracy predicting healthy loans, 87% accuracy predicting high-risk loans
- Accuracy: 94% balanced accuracy score
- Recall: 100% recall for healthy loans, 89% recall for high-risk loans

### Logistic Regression Model 2:

- Precision: 100% accuracy predicting healthy loans, 87% accuracy predicting high-risk loans
- Accuracy: 99% balanced accuracy score
- Recall: 100% recall for healthy loans, 100% recall for high-risk loans

## Summary
Overall the second Logistic Regression Model performs the best with balanced oversampled data, we see accuracy increase slightly and the number of false negatives decrease drastically; however, we also see false positives increase. The better place to start could be with a model fitted with balanced data, or balanced oversampled data that originally didn't have such a massive classification imbalance as this dataset.
