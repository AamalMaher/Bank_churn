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


<p>The model was fine-tuned using GridSearch to optimize the hyperparameters, ensuring the best possible performance for the stacking ensemble.</p>

<h3>Models Used in Stacking:</h3>
<ul>
    <li>Base models (e.g., Logistic Regression, Decision Trees, Random Forest, etc.)</li>
    <li>Meta-model: Combines predictions from base models for the final output.</li>
</ul>

<h2>Deployment</h2>
<p>The model is deployed using <strong>Streamlit</strong>, providing an interactive web interface for real-time churn predictions.</p>

<h2>Installation and Setup</h2>
<ol>
    <li><strong>Clone the repository</strong>:
        <pre><code>git clone &lt;repository-url&gt;
        <h2>Usage</h2>
<p>Open the Streamlit app in your browser. Input customer details such as Credit Score, Age, Balance, etc., and click <strong>Predict</strong> to get the churn prediction (Yes/No).</p>

<h2>Files</h2>
<ul>
    <li><code>app.py</code>: Streamlit application file.</li>
    <li><code>stacking_model.pkl</code>: Pre-trained stacking model saved with <code>joblib</code>.</li>
    <li><code>requirements.txt</code>: Python package requirements.</li>
</ul>

<h2>Results</h2>
<p>The stacking model achieved an accuracy of <strong>84%</strong> on the test data.</p>

