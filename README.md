# Instruction
The dataset contains commercial customers' financial information and default status within the next 12 months. The goal is to build a binary classifier to predict customers default probability.

1. Load both training and testing sets.
2. Winsorize "feature_1" and "feature_3" by limiting the extreme values to 1 percentile (left tail) and 99 percentile (right tail).
3. Identify the missing values in the dataframe. Then, fill the missings with median value.
4. Standardize "feature_1", "feature_2", "feature_3", "feature_4".
5. Build a logistic regression on the train set to predict 'y' using "feature_1", "feature_2", "feature_3", "feature_4" as independent variables.
6. Report AUC on testing set.
7. Report confusion matrix on testing set.
