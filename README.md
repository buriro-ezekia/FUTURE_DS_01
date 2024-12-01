# FUTURE_DS_01
# Titanic Survival Prediction
1. **Understand the Problem**
- Objective: Predict survival on the Titanic based on passenger data.
- Key Output: A submission file with predictions (**0** for not survived and **1** for survived).
- Evaluation Metric: Accuracy of predictions.

In this project, I worked on predicting passenger survival on the Titanic by leveraging data analysis and machine learning techniques. I started with an in-depth exploration of the dataset, inspecting its structure and summarising its contents. During this phase, I identified missing values and examined the distribution of features to understand the data. Addressing the missing data was an important step; I employed strategies like filling or dropping missing values for columns such as **Age** and **Cabin**, ensuring the data was clean and ready for analysis.

Feature engineering played a vital role in shaping the dataset for model training. I transformed categorical variables into a suitable format using one-hot encoding. Moreover, I created new features that could enhance predictive performance. Additionally, I used a Random Forest algorithm to assess feature importance, which guided me in selecting the most relevant features for my models. This step included variables like **Sex_male**, **Fare**, **PassengerId**, **Age**, and **Pclass_3**, ensuring that only impactful data contributed to the model.

Model training explored multiple algorithms, including **Logistic Regression**, **Random Forest**, and **Gradient Boosting**. I used a validation set to evaluate their performance and measure effectiveness on metrics, including accuracy, precision, recall, and F1 score. After evaluation, I opted for the **Gradient Boosting** model due to its strong performance and ability to capture complex relationships between features, making it well-suited for this problem.

Once I trained and validated the model, I applied the same preprocessing steps to the test dataset to ensure consistency. Using the trained Gradient Boosting model, I predicted survival outcomes for the 418 passengers in the test set. The predictions are formatted into a CSV file containing the PassengerId and Survived columns for submission and further analysis.

This project has provided valuable experience with data preprocessing, feature engineering, and model evaluation and demonstrated the effectiveness of ensemble models like Gradient Boosting in making reliable predictions on complex datasets.
