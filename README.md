# Loan-Approval-Prediction
Overview
This project aims to predict loan approval status using various applicant features. The dataset includes information such as income, loan amount, credit history, and other relevant attributes. Additionally, the project provides insights into the reasons for loan rejections through an interactive visualization.

Table of Contents
Dataset
Modeling
Evaluation
Rejection Analysis
Interactive Visualization
Usage
Requirements
Contributing
License
Dataset
The dataset used in this project contains the following columns:

Loan_ID: Unique identifier for each loan application.
Gender: Gender of the applicant.
Married: Marital status of the applicant.
Dependents: Number of dependents.
Education: Education status of the applicant.
Self_Employed: Whether the applicant is self-employed.
ApplicantIncome: Income of the applicant.
CoapplicantIncome: Income of the co-applicant.
LoanAmount: Amount of loan requested.
Loan_Amount_Term: Duration of the loan in months.
Credit_History: Credit history status.
Property_Area: Area of the property.
Loan_Status: Status of the loan (0 = Not Approved, 1 = Approved).
Modeling
The following steps were followed to create the loan approval prediction model:

Data Preprocessing:

Handle missing values.
Encode categorical features.
Normalize numerical features.
Model Selection:

Used Random Forest Classifier for its robustness and accuracy.
Training and Testing:

Split the dataset into training and testing sets.
Fit the model and make predictions.
Evaluation
The model performance was evaluated using:

Accuracy: Measures the proportion of correct predictions.
Confusion Matrix: Shows the breakdown of true positives, true negatives, false positives, and false negatives.

Classification Report: Provides precision, recall, and F1-score for each class.
Example Output
plaintext
Copy code
Accuracy: 0.8229
Confusion Matrix:
[[14 14]
 [ 3 65]]
Classification Report:
              precision    recall  f1-score   support

           0       0.82      0.50      0.62        28
           1       0.82      0.96      0.88        68
Rejection Analysis
To provide transparency to applicants, the project includes an analysis of the reasons for loan rejections. Key insights include:

Rejection Criteria: The model identifies and presents common characteristics among applicants who were not approved for loans.
Reasons for Rejection: Common factors influencing loan denials, such as low income, high loan amounts compared to income, or poor credit history.
These insights can help applicants understand their loan eligibility better and improve their chances in future applications.

Interactive Visualization
An interactive bar chart shows the reasons for loan rejections, allowing users to explore the reasons based on various criteria. The visualization was created using Plotly.

Visualization Features
Hover over bars to see detailed counts.
Filtered to only show rejected loans and their respective reasons.
Usage
Clone the repository.
Install the required packages using:
bash
Copy code
pip install -r requirements.txt
Run the notebook or script to execute the model and generate the visualization.
Requirements
Python 3.7+
Pandas
NumPy
scikit-learn
Plotly
Contributing
Feel free to open issues or submit pull requests. Contributions are welcome!

License
This project is licensed under the MIT License. See the LICENSE file for details.

