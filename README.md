# Customer-Churn-Retention-and-Analysis-Based-Business-Decision

The project is centered around analyzing customer churn, a key metric for businesses that want to minimize customer loss. The primary objective was to build a predictive model to identify customers likely to leave, enabling the creation of targeted retention strategies.

### Step-by-Step Project Description

1. **Data Collection & Import**: 
   - Customer data was loaded, with a focus on churn-related features such as contract length, payment method, monthly charges, and tenure.

2. **Data Cleaning**:
   - Converted data types for numerical consistency.
   - Checked for missing values and duplicates, ensuring that the dataset was accurate and complete.
   - Imputed missing values in `TotalCharges` and addressed outliers in columns like `tenure` and `MonthlyCharges` to improve model reliability.

3. **Feature Engineering**:
   - **Categorical Encoding**: Used one-hot encoding to transform categorical variables (e.g., `gender`, `Contract`, `PaymentMethod`) into binary columns, preparing them for model training.
   - **Scaling**: Standard scaling was applied to numerical data, ensuring that features were on a comparable scale, which benefits algorithms like Logistic Regression.

4. **Exploratory Data Analysis (EDA)**:
   - Visualizations helped explore the distribution of features and their relationship with churn. For example, analyzing patterns in `tenure` and `MonthlyCharges` between churned and retained customers can highlight high-risk groups.
   - Correlation analysis and skewness metrics helped identify influential features.

5. **Model Training & Evaluation**:
   - **Model Choice**: Logistic Regression was used to predict churn, with a 70-30 train-test split. The model's performance was evaluated using a confusion matrix and accuracy score, providing a baseline for identifying high-risk customers.
   
6. **Deployment Preparation**:
   - Code snippets suggest steps for deploying the model via FastAPI and Streamlit, making the predictive insights accessible in real-time for customer management teams.

### Key Findings

With the model’s accuracy in identifying potential churn, several customer trends can be observed:
- **High Churn Correlations**: Higher monthly charges and shorter tenure were likely associated with increased churn.
- **Contract Type Influence**: Customers with month-to-month contracts might exhibit a higher churn risk than those with long-term contracts.

### Customer Retention Strategies

1. **Contract Incentives**:
   - Offer long-term contract discounts or perks to customers with month-to-month contracts, potentially increasing retention among short-term contract users.

2. **Targeted Discounts for High Charges**:
   - For customers with high monthly charges, implement a rewards program or offer tiered discounts, reducing the likelihood of these customers leaving due to cost.

3. **Enhanced Customer Support for New Customers**:
   - Since lower tenure is a strong churn indicator, prioritize engaging with new customers through personalized support, onboarding, and check-ins during their first few months.

4. **Customized Retention Outreach**:
   - Use the model predictions to identify at-risk customers, then design proactive campaigns (like email or SMS alerts) to re-engage them.

5. **Feedback Loop Implementation**:
   - Collect feedback from customers identified as high risk and analyze it for actionable insights. This will help continuously refine retention strategies and improve customer satisfaction.

--- 
