# Bank Churn Prediction

![Banner Image](https://miro.medium.com/v2/resize:fit:1400/0*8Iu_eymr6eR-YuQw)  <!-- Replace with the URL of your banner image -->

## Project Overview

The Bank Churn Prediction project aims to predict customer churn in a banking context. Churn prediction helps banks understand which customers are likely to leave their services, allowing them to take proactive measures to retain valuable clients.

### Key Features:
- **Credit Score**: Customer's credit rating.
- **Geography**: Country where the customer resides.
- **Gender**: Customer's gender.
- **Age**: Customer's age.
- **Tenure**: Duration the customer has been with the bank.
- **Balance**: Customer's account balance.
- **NumOfProducts**: Number of products the customer has with the bank.
- **HasCrCard**: Indicator of whether the customer has a credit card.
- **IsActiveMember**: Indicator of whether the customer is an active member.
- **EstimatedSalary**: Customer's estimated salary.
- **Exited**: Target variable indicating whether the customer exited (1) or not (0).

## Data Preprocessing

### Data Cleaning
1. **Removal of Irrelevant Columns**:
   - Dropped `RowNumber` and `CustomerId` as they do not provide predictive value.
   - Dropped `Surname` as it is not relevant for prediction.

2. **Handling Missing Values**:
   - The dataset does not have missing values.

### Feature Encoding
1. **Categorical Encoding**:
   - Converted `Gender` to numeric values (Female: 1, Male: 0).
   - Applied one-hot encoding to the `Geography` column to transform categorical values into numerical format.

2. **Feature Scaling**:
   - Applied Min-Max Scaling to features such as `Age`, `Tenure`, `CreditScore`, `Balance`, and `EstimatedSalary` to normalize the data.
   - Scaled `NumOfProducts` to ensure all features are on a similar scale.

### Data Transformation
- The dataset was transformed into a format suitable for machine learning models by scaling numerical features and encoding categorical variables.

## Model Building

The model building process involved several steps:
1. **Data Splitting**:
   - The dataset was split into training and test sets to evaluate model performance.

2. **Model Selection**:
   - Various classification models were considered for predicting customer churn, including Logistic Regression, Random Forest, and Gradient Boosting.

3. **Model Training**:
   - The selected models were trained on the processed dataset.

4. **Evaluation**:
   - Models were evaluated using metrics such as accuracy, precision, recall, and F1-score.

5. **Results**:
   - The best-performing model was selected based on evaluation metrics and applied to make predictions on unseen data.

## Visualization

Visualizations were used to understand the data better and to identify patterns:
- **Balance Distribution**: Compared account balances between customers who exited and those who did not to gain insights into the relationship between account balance and churn.

## Conclusion

The project demonstrates the use of machine learning techniques to predict customer churn in a banking context. By preprocessing data effectively and applying various models, we aim to provide actionable insights for customer retention strategies.

## Future Work

- **Model Improvement**: Experiment with more advanced algorithms and hyperparameter tuning.
- **Additional Features**: Incorporate more features that might affect customer churn.
- **Deployment**: Develop a user interface to make predictions in real-time.

## References

- Dataset: [Bank Churn Dataset](https://example.com/dataset)  <!-- Replace with the URL or reference to the dataset -->

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
