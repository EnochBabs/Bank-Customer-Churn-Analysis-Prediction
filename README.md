# Bank-Customer-Churn-Analysis-Prediction

## Project Overview
This project analyzes and predicts customer churn for a bank using machine learning techniques. By identifying factors that influence customer decisions to leave the bank, we aim to help develop effective retention strategies.

## Dataset
The dataset contains 10,000 customer records with the following features:
- **CustomerId**: Unique identifier for the customer
- **Surname**: Customer's last name
- **CreditScore**: Customer's credit score
- **Geography**: Customer's location (France, Spain, etc.)
- **Gender**: Customer's gender
- **Age**: Customer's age
- **Tenure**: Number of years the customer has been with the bank
- **Balance**: Customer's account balance
- **NumOfProducts**: Number of bank products the customer is using
- **HasCrCard**: Whether the customer has a credit card (1=Yes, 0=No)
- **IsActiveMember**: Whether the customer is an active member (1=Yes, 0=No)
- **EstimatedSalary**: Customer's estimated salary
- **Exited**: Whether the customer left the bank (1=Yes, 0=No) - Target variable

## Project Structure
The analysis follows these steps:
1. **Data Loading and Exploration**: Initial examination of data characteristics
2. **Exploratory Data Analysis**: Visualization of key relationships and distributions
3. **Feature Engineering**: Preparing features for modeling
4. **Model Building**: Training classification models to predict churn
5. **Model Evaluation**: Assessing model performance
6. **Hyperparameter Tuning**: Optimizing model parameters
7. **Customer Segmentation**: Identifying key customer segments by churn risk

## Key Findings
- Customer age shows a strong relationship with churn rates
- Geography plays a significant role in churn behavior
- The Random Forest classifier outperforms Logistic Regression (86.7% vs 81.1% accuracy)
- Class imbalance affects model performance, with lower recall for the minority (churned) class
- Older customers (>60 years) have significantly higher churn rates

## Model Performance
The Random Forest classifier achieved:
- Accuracy: 86.7%
- Precision for churn prediction: 76%
- Recall for churn prediction: 47%

## How to Use This Project
1. Clone the repository
2. Install the required dependencies:
   ```
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Run the Jupyter notebook:
   ```
   jupyter notebook bank_churn_prediction.ipynb
   ```

## Future Improvements
- Implement techniques to address class imbalance (SMOTE, class weights)
- Try additional feature engineering for improved predictive power
- Explore more advanced algorithms like XGBoost or neural networks
- Adjust probability thresholds to improve recall for the minority class
- Develop a customer retention strategy based on model insights

## Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Contact
For questions or feedback, please contact enochferanni@gmail.com
