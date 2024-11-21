# Fraud Detection Using XGBoost  

## 📖 Overview  
This project demonstrates the application of **XGBoost** to detect fraudulent transactions. It involves feature engineering, data preprocessing, hyperparameter optimization, and model evaluation using metrics like AUC-ROC, classification report, and confusion matrix.  

## 🚀 Key Features  
- **Feature Engineering**: Created additional features such as `transaction_diff`, `recipient_diff`, and a binary flag for large transactions.  
- **Hyperparameter Optimization**: Tuned the XGBoost model using `RandomizedSearchCV` for better performance.  
- **Evaluation Metrics**: Used AUC-ROC, classification report, and feature importance analysis.  
- **Visualization**: Barplot of feature importance for model interpretability.  

---

## 🛠️ Installation  

### Requirements  
Ensure you have the following libraries installed:  
- `pandas`  
- `numpy`  
- `scikit-learn`  
- `xgboost`  
- `matplotlib`  
- `seaborn`  
- `scipy`  

Install the required libraries using pip:  

pip install pandas numpy scikit-learn xgboost matplotlib seaborn scipy
📂 Data Description

The dataset contains information on financial transactions with the following key fields:

amount: Transaction amount.
oldbalanceOrg: Initial balance in the origin account.
newbalanceOrig: Balance after the transaction in the origin account.
oldbalanceDest: Initial balance in the destination account.
newbalanceDest: Balance after the transaction in the destination account.
type: Type of transaction (e.g., CASH-IN, TRANSFER).
isFraud: Target variable indicating if the transaction is fraudulent.


## 🖥️ Usage

### Clone the repository:
git clone https://github.com/praneethsattavaram/Fraud-Detection-Using-XGBoost.git
### Navigate to the project directory:
cd Fraud-Detection-Using-XGBoost
Place the dataset Fraud.csv in the project directory.
### Run the script:
python main.py


## 📊 Model Workflow

### Data Preprocessing:
Handled missing values for destination account balances.
Generated new features for better predictive power.
Encoded categorical features using one-hot encoding.
Scaled numerical features using StandardScaler.
### Model Training:
Used XGBoost for classification.
Performed hyperparameter tuning with RandomizedSearchCV.
Evaluation:
Evaluated the model using AUC-ROC, classification report, and confusion matrix.
Plotted feature importance for model interpretability.


## 🛠️ Key Results

### Best Hyperparameters:
The script outputs the best hyperparameters identified through random search.
### Model Metrics:
AUC-ROC: Measures the model's ability to differentiate between fraudulent and legitimate transactions.
Confusion Matrix: Summarizes the prediction performance.
### Feature Importance:
Identifies the most critical features influencing the prediction.


## 📜 License

This project is licensed under the MIT License.

## 🙌 Acknowledgments

 XGBoost: For its robust and efficient gradient boosting framework.
 Scikit-learn: For tools and utilities for preprocessing and evaluation.
Matplotlib & Seaborn: For visualizations.
📬 Contact

### For any queries or suggestions, please reach out:
Email: praneethsattavaram@gmail.com
