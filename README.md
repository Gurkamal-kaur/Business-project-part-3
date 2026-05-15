# 📌 Project Title  
Customer Churn Prediction using Machine Learning  

# 🛒 Business Problem  
The company wants to identify customers who are likely to stop using its services. By predicting churn, the business can take proactive steps to retain valuable customers, reduce revenue loss, and design targeted retention campaigns.  

# 📂 Dataset Source  
- Name: Customer Churn Dataset  
- Origin: Google Drive (shared dataset)  
- Direct Download Link: https://drive.google.com/uc?id=1Gn9-RV7YzH3hJFKd2CO39hMOs83li9Tx  

# 📑 Dataset Description  
- Size: ~7,000 rows  
- Columns: CustomerID, Gender, SeniorCitizen, Partner, Dependents, Tenure, PhoneService, InternetService, Contract, PaymentMethod, MonthlyCharges, TotalCharges, Churn  
- Granularity: Each row represents one customer’s profile and subscription details  

# 🛠️ Tools and Libraries Used  
- Python (Google Colab / Jupyter Notebook)  
- pandas, numpy → data preprocessing & feature engineering  
- matplotlib, seaborn → visualizations  
- scikit‑learn → model building & evaluation  

# 🔎 Steps Performed  
1. Data Understanding  
2. Data Cleaning & Preprocessing  
3. Exploratory Data Analysis (EDA)  
4. Feature Engineering  
5. Model Building (Logistic Regression, Random Forest, XGBoost)  
6. Model Evaluation (Accuracy, Precision, Recall, F1‑Score, ROC‑AUC)  
7. Business Recommendations  

# 🧹 Data Cleaning Summary  
- Handled missing values in `TotalCharges`  
- Converted categorical variables into numerical (Label Encoding / One‑Hot Encoding)  
- Standardized numerical features (`MonthlyCharges`, `TotalCharges`, `Tenure`)  
- Removed duplicates  

# 📊 EDA Insights  
- Customers with **month‑to‑month contracts** churn more often than those with long‑term contracts  
- **High monthly charges** are strongly associated with churn  
- **Electronic check payment method** customers show higher churn rates  
- Senior citizens and customers with no dependents are more likely to churn  

# 🤖 Modeling Approach  
- Split dataset into train/test sets (80/20)  
- Applied multiple models: Logistic Regression, Random Forest, XGBoost  
- Compared performance using ROC‑AUC and F1‑Score  
- Best performing model: **Random Forest (ROC‑AUC ~0.85)**  

# 🧩 Model Interpretation  
- **High Risk Customers**: Month‑to‑month contracts, high charges, electronic check payments  
- **Low Risk Customers**: Long‑term contracts, auto‑payment, lower charges  
- **Moderate Risk Customers**: Mid‑range tenure, moderate charges  

# 💡 Final Business Recommendations  
- High Risk: Offer discounts on long‑term contracts, personalized retention calls  
- Moderate Risk: Provide loyalty rewards, upsell bundled services  
- Low Risk: Maintain satisfaction with exclusive perks and engagement programs  

# ▶️ How to Run the Project  
Clone the repository and install requirements:  
```bash
git clone https://github.com/Gurkamal-kaur/customer-churn-prediction.git
cd customer-churn-prediction
pip install -r requirements.txt
