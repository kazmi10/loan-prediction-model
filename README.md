 # Loan Default Prediction Model

## Project Overview
This project involves building a machine learning model to predict whether a loan applicant will default on their loan. The model is built using a RandomForestClassifier and is tuned to achieve the best possible accuracy.

## Dataset
The dataset used in this project includes information about applicants, such as their income, loan amount, credit history, and more. The target variable is `Loan_Status`, which indicates whether a loan was approved ('Y') or not ('N').

## Methodology
1. **Data Preprocessing:**
   - Handled missing values using median for numerical features and mode for categorical features.
   - Applied one-hot encoding to categorical variables.

2. **Modeling:**
   - Split the data into training and validation sets.
   - Trained a RandomForestClassifier and performed hyperparameter tuning using Grid Search.

3. **Evaluation:**
   - Achieved a cross-validation accuracy of 82.28% with the best parameters.
   - Evaluated the model using accuracy, confusion matrix, and classification report.

4. **Final Predictions:**
   - Used the tuned model to make predictions on the test set.
   - Prepared and saved the submission file.

## Results
- **Best Cross-Validation Accuracy:** 82.28%
- **Validation Accuracy with Best Parameters:** (Include your validation accuracy here)

## How to Run the Project
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/kazmi10/loan-prediction-model.git
2. Install Dependencies:
   pip install -r requirements.txt
3. Run the Notebook:
Open and run the Jupyter notebook Loan_Prediction_Model.ipynb.

Future Work
Experiment with other models such as XGBoost or LightGBM.
Implement advanced feature engineering techniques.
Explore the use of deep learning for more complex patterns.


#### **11.2 Clean Up Your Jupyter Notebook**

Make sure your Jupyter Notebook is clean, well-commented, and easy to follow. Here’s what to do:

- **Remove Unnecessary Cells:** Remove any redundant or debugging cells.
- **Add Markdown Cells:** Use markdown cells to explain each section of the notebook.
- **Ensure Clear Outputs:** Ensure that the output cells are clear and informative.

#### **11.3 Prepare the Submission File**

Ensure your submission file (`final_loan_prediction_submission.csv`) is correctly formatted and ready for submission.

### **Step 12: Upload to GitHub**

If you want to share your work, create a GitHub repository for your project.

#### **12.1 Create a GitHub Repository**

1. **Go to GitHub:**
   - Log in to your GitHub account and click on the “New repository” button.

2. **Name the Repository:**
   - Give your repository a meaningful name, such as `loan-prediction-model`.

3. **Initialize with a README:**
   - Check the option to initialize the repository with a README file.

4. **Add Files:**
   - Upload your Jupyter notebook (`.ipynb` file), the dataset (if permissible), and the final submission file.
   - Add the `README.md` file and any other necessary files, like a `requirements.txt` if you used specific Python packages.

#### **12.2 Commit and Push Changes**

If you’re working locally with Git, you can commit your changes and push them to GitHub.

 ## Results

### Model Performance
- **Best Cross-Validation Accuracy:** 82.28%
  - After performing Grid Search for hyperparameter tuning, the best model achieved a cross-validation accuracy of 82.28%. This indicates that the model is likely to generalize well to unseen data.

### Validation Set Performance
- **Validation Accuracy:** 76.76%
  - The model achieved an accuracy of 76.76% on the validation set. This reflects the model's performance on data it hadn't seen during training and is a good indicator of how it might perform on the test set.

### Detailed Metrics
- **Precision, Recall, and F1-Score:**
  - **Class 1 (Loan Approved):**
    - **Precision:** 0.76
    - **Recall:** 0.94
    - **F1-Score:** 0.84
  - **Class 0 (Loan Not Approved):**
    - **Precision:** 0.81
    - **Recall:** 0.45
    - **F1-Score:** 0.57
  - The model shows strong performance in identifying loan approvals, with high precision and recall for Class 1. However, it struggles more with identifying loans that should not be approved (Class 0), where recall is lower.

### Final Observations
- The model is well-calibrated for predicting loan approvals but might benefit from further tuning or the use of alternative algorithms to improve recall for non-approvals. This could involve balancing the dataset or exploring more complex models like XGBoost or ensemble methods.

