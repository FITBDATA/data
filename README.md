# Instruction
The panel dataset contains commercial customers' financial information and days past due indicator from 2000 to 2020. The goal is to build a binary classifier to predict customers default probability. 

1. Load both training and testing sets.
2. Winsorize **"feature_1"** and **"feature_3"** by limiting the extreme values to 1 percentile (left tail) and 99 percentile (right tail).
3. Identify missing values for **"feature_3"**. Then, impute the missings with median value.
4. Identify missing values for **"feature_2"**. Then, for each **"id"**, impute the missings with the value from previous year, if not available, use the value from next year.
5. Standardize **"feature_1"**, **"feature_2"**, **"feature_3"**, **"feature_4"**.
6. Build a logistic regression on the training set to predict **'y'** using **"feature_1"**, **"feature_2"**, **"feature_3"**, **"feature_4"** as independent variables.
7. Report AUC on testing set.
8. Report confusion matrix on testing set.
