<h2>Overview</h2>
<p>This project predicts customer churn (i.e., whether a customer will leave the bank) using a stacking ensemble model. The predictive model is deployed using Streamlit for user interaction.</p>

<h2>Features</h2>
<ul>
    <li><strong>CreditScore</strong>: Customer's credit score.</li>
    <li><strong>Geography</strong>: Customer's country (e.g., France, Spain, Germany).</li>
    <li><strong>Gender</strong>: Customer's gender (Male/Female).</li>
    <li><strong>Age</strong>: Customer's age.</li>
    <li><strong>Tenure</strong>: Number of years the customer has been with the bank.</li>
    <li><strong>Balance</strong>: Customer's account balance.</li>
    <li><strong>NumOfProducts</strong>: Number of bank products the customer uses.</li>
    <li><strong>HasCrCard</strong>: Indicates if the customer has a credit card (0 = No, 1 = Yes).</li>
    <li><strong>IsActiveMember</strong>: Indicates if the customer is an active member (0 = No, 1 = Yes).</li>
    <li><strong>EstimatedSalary</strong>: Customer's estimated salary.</li>
    <li><strong>Exited</strong>: Target column indicating whether the customer has exited the bank (0 = No, 1 = Yes).</li>
</ul>


## Steps  

1. **Data Preprocessing**  
   - Cleaned the data by handling missing values and inconsistencies.  
   - Encoded categorical variables (e.g., Geography, Gender) to prepare them for model training.  

2. **Model Training**  
   - Used the **Stacking Model** to train the model with the training data.  

3. **Hyperparameter Tuning**  
   - Tuned hyperparameters of the XGBoost model using **GridSearchCV** to achieve optimal performance.  

4. **Evaluation**  
   - Evaluated the model using metrics such as **AUC**, **Confusion Matrix**, and a **classification report** to ensure high accuracy.  

<h3>Models Used in Stacking:</h3>
<ul>
    <li>Base models (e.g., Logistic Regression, Decision Trees, Random Forest, etc.)</li>
    <li>Meta-model: Combines predictions from base models for the final output.</li>
</ul>

