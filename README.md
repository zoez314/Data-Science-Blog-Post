# Loan Repayment Analysis  

## Project Motivation  
This project explores loan repayment behavior using a dataset of **9,578 loan records**. The motivation is to identify key factors influencing defaults, compare loan repayment probabilities across different purposes, and evaluate predictive models to assist lenders in making informed decisions.  

---

## Libraries Used  
The following Python libraries were used for data analysis, visualization, and modeling:  
- **pandas**: Data manipulation and analysis.  
- **numpy**: Numerical computations.  
- **matplotlib**: Data visualization.  
- **seaborn**: Statistical data visualization.  
- **scikit-learn**: Machine learning modeling and evaluation.  

---

## Repository Structure  

```plaintext  
├── loan_data.csv                   # Dataset file  
├── Data_Scientist_Blog_Post.ipynb  #Jupyter Notebook for data analysis and modeling  
├── README.md                       # Documentation of the project  
├── requirements.txt                # List of dependencies for the project  

```
# Summary of Results

## Key Findings:

### Factors Affecting Defaults:
- **Higher interest rates** and **debt-to-income ratios** increase the likelihood of default.
- **Lower FICO scores** are strongly associated with defaults.

### Role of FICO Scores:
- Borrowers with **FICO scores below 700** are **20% more likely to default** than those with scores above 700.

### Loan Purpose and Default Rates:
- Loans for **small businesses** have the highest default rate (**~25%**), while **debt consolidation loans** show moderate default rates (**~15%**).

### Model Comparison:
- **Random Forest** outperforms Logistic Regression:
  - Achieves an accuracy of **83%**.
  - Successfully identifies **78% of defaulters**.

---

## Files in the Repository:

- **`loan_repayment_analysis.ipynb`**: Jupyter Notebook containing all the analysis and modeling steps.
- **`requirements.txt`**: A list of Python dependencies required to run the project.