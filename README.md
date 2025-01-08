# 🚀 Loan Default Prediction Using Logistic Regression 📚

## Overview
This project implements a Logistic Regression model to predict whether a loan applicant will default based on features such as loan amount, income, interest rate, and more. The data is preprocessed and split into training and testing sets before being used for model training.

## 🔧 Installation

### Clone the repository to your local machine:
```bash
git clone https://github.com/zoez314/Data-Science-Blog-Post.git

##Install the required dependencies:

pip install -r requirements.txt

#🧑‍💻 Features
Data Preprocessing: Missing value handling, scaling, encoding categorical variables.
Model Training: Logistic Regression model.
Evaluation: Confusion matrix, accuracy score, and ROC curve.
Hyperparameter Tuning: Grid search for optimal parameters.
#📊 Visualizations
Correlation Matrix 🔄: Shows relationships between numerical features.
Pairplot 🔍: Helps visualize distributions and pairwise relationships between features.
⚙️ Steps to Run the Model
#1. Preprocess Data 🧹
Clean and scale the data to prepare it for training. We use StandardScaler to standardize numerical features for better model performance.

#2. Train the Logistic Regression Model ⚙️
from sklearn.linear_model import LogisticRegression
from sklearn.preprocessing import StandardScaler

# Scale the data
scaler = StandardScaler()
X_train_scaled = scaler.fit_transform(X_train)
X_test_scaled = scaler.transform(X_test)

# Train the model
model = LogisticRegression(max_iter=2000)
model.fit(X_train_scaled, y_train)

# Make predictions
y_pred = model.predict(X_test_scaled)

#3. Model Evaluation 📈
Evaluate model performance using metrics like accuracy, confusion matrix, and ROC curve.

#⚠️ Warnings
If you encounter the following warning during model training:
ConvergenceWarning: lbfgs failed to converge...

You can solve it by:

Increasing the number of iterations (max_iter=2000).
Scaling the features using StandardScaler.

#📝 License
This project is licensed under the MIT License - see the LICENSE file for details.
