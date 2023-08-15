<img width="760" alt="Screenshot 2023-08-15 at 1 11 47 AM" src="https://github.com/P4RASTOO/Challenge_13/assets/132952512/6adf6def-d456-4a9a-a833-2b079ca9383f">

# Challenge_13 Report
## Overview of the Analysis
The purpose of this analysis was to develop and evaluate machine learning models for predicting the success of funding applications received by Alphabet Soup, a venture capital firm. The goal was to create a predictive model that assists in determining whether startups would become successful businesses if funded by Alphabet Soup.

Financial Information and Prediction Target:
The dataset contained information about more than 34,000 organizations that received funding from Alphabet Soup. The data included features such as APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, and IS_SUCCESSFUL. The variable of interest for prediction was IS_SUCCESSFUL, which indicated whether an applicant became a successful business after receiving funding.

## Stages of the Machine Learning Process:
1) Data Preprocessing: The dataset was loaded, and categorical variables were encoded using techniques like one-hot encoding. The features were scaled using standardization to ensure uniformity in model training.
Model Selection: Various machine learning models were considered, including Decision Trees, Random Forests, and Neural Networks. Models were selected based on their suitability for binary classification tasks and their potential to capture complex relationships in the data.

2) Feature Importance Analysis: For Random Forests, feature importance analysis was performed to identify the most influential features in predicting success. This helped in feature selection and provided insights into which variables were most relevant for the prediction task.
Hyperparameter Tuning: Grid search was employed to optimize hyperparameters for the neural network model. Different combinations of hyperparameters were tested to find the best configuration that maximized model performance.

3) Model Evaluation: Each model's performance was evaluated using evaluation metrics such as accuracy, loss, and possibly other relevant metrics. The models were trained on the training dataset and then evaluated on the separate testing dataset to assess their ability to generalize to new, unseen data.

4) Results and Comparison: The results of all models, including the original and alternate neural network models, were compiled and compared. The evaluation metrics provided insights into how well the models performed in predicting successful businesses.

## Methods Used:
In this analysis, various machine learning methods were utilized, including:

Neural Networks: Employed for their capacity to capture intricate patterns in the data. Hyperparameter tuning and feature selection were performed to optimize neural network performance.

Overall, the analysis aimed to develop accurate predictive models that can assist Alphabet Soup in making informed decisions about funding applications, ultimately contributing to the success of startups.

## Summary
Summary of the results of the machine learning models and a recommendation based on their performance:
### Original Model:

* Loss: 0.552234
* Accuracy: 0.732945
  
The original model is a neural network with a relatively simple architecture. While it has a moderate accuracy of approximately 73.3%, its loss is relatively high compared to the alternate models. This might suggest that the model struggles to generalize well to the data, possibly due to its simplicity.

### Alternate Model 1:

* Loss: 0.186438
* Accuracy: 0.731895
  
Alternate Model 1 is another neural network with a different architecture. It has a significantly lower loss compared to the original model and a similar accuracy. The lower loss indicates that this model better fits the training data and likely performs better on unseen data. However, the relatively modest accuracy suggests that there might be room for improvement.

### Alternate Model 2:

* Loss: 0.557254
* Accuracy: 0.731429
  
Alternate Model 2 is a more complex neural network with additional dropout layers. While it has a higher loss and similar accuracy compared to the original model, the increased complexity of the architecture may contribute to overfitting.

## Recommendation:
Based on the evaluation results, it appears that Alternate Model 1 performs the best among the three models. It has a lower loss than both the original model and Alternate Model 2, indicating better generalization to new data. While the accuracy is similar across all models, the lower loss of Alternate Model 1 suggests that it is a more suitable choice for predicting the success of funding applications.

Therefore, the recommendation is to use Alternate Model 1 for predicting whether applicants will be successful if funded by Alphabet Soup. However, further fine-tuning and optimization of the model's hyperparameters and architecture could potentially lead to even better performance.


