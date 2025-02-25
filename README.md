# Max-Life-Health-Insurance-Cross-Sell-Prediction

### **Introduction**
In the insurance industry, companies want to identify customers who might buy additional policies. This project, **Max Life Health Insurance Cross-Sell Prediction**, uses machine learning to predict if a customer is likely to purchase health insurance. By analyzing past data, we can create a model that helps the company improve marketing and increase sales.

### **Problem Statement**
Many insurance companies struggle to find the right customers for additional policies. Traditional marketing methods often waste resources and time. This project aims to build a machine learning model to predict which customers are interested in buying health insurance, making marketing more effective.

### **Dataset Overview**
The dataset has **381,109 records** with **12 features**, including customer details, past insurance history, and vehicle-related information. Key features include:
- **Gender**: Male or Female
- **Age**: Customer's age in years
- **Driving_License**: If the customer has a driving license (1 = Yes, 0 = No)
- **Region_Code**: Location of the customer
- **Previously_Insured**: If the customer already has an insurance policy (1 = Yes, 0 = No)
- **Vehicle_Age**: How old the vehicle is (<1 Year, 1-2 Years, >2 Years)
- **Vehicle_Damage**: If the vehicle was damaged before (Yes/No)
- **Annual_Premium**: Insurance cost paid by the customer
- **Policy_Sales_Channel**: How the policy was sold
- **Vintage**: How long the customer has been with the company
- **Response (Target Variable)**: If the customer is interested in buying health insurance (1 = Yes, 0 = No)

### **Methodology**
This project follows a step-by-step approach to build a predictive model:

#### **1. Exploratory Data Analysis (EDA)**
We first analyze the dataset to understand trends, check for missing values, and find important patterns. Some key insights include:
- Age groups more likely to buy insurance
- The impact of vehicle damage history on interest
- How policy sales channels influence customer decisions

#### **2. Data Preprocessing**
To clean and prepare data for the model, we:
- Convert text data (like `Vehicle_Age` and `Gender`) into numbers
- Scale numerical values like `Annual_Premium`, `Vintage`, and `Age`
- Remove unnecessary columns, such as `id`

#### **3. Feature Engineering**
To improve model accuracy, we create new features like:
- **Insurance Score**: Based on `Previously_Insured`, `Vehicle_Damage`, and `Annual_Premium`
- **Customer Loyalty Index**: Using `Vintage` and `Region_Code`

#### **4. Model Selection and Training**
We test different machine learning models to find the best one:
- **Logistic Regression** (Basic model)
- **Random Forest** (Good for handling different types of data)
- **Gradient Boosting (XGBoost, LightGBM, CatBoost)** (Best for large datasets)
- **Neural Networks** (If deep learning is needed)

#### **5. Model Evaluation**
We measure model performance using:
- **Accuracy**: How many predictions are correct
- **Precision & Recall**: Balancing false positives and false negatives
- **F1 Score**: A combined accuracy measure
- **AUC-ROC**: Measures how well the model distinguishes between interested and not-interested customers

#### **6. Model Optimization & Hyperparameter Tuning**
We fine-tune the model using techniques like Grid Search and Random Search to improve accuracy.

#### **7. Deployment (Optional)**
Once the model is ready, we can deploy it using:
- **Streamlit**: For a simple web application
- **Flask/Django API**: To integrate with company systems

### **Expected Outcomes**
By the end of this project, we will:
- Create an accurate model to predict customer interest in health insurance
- Provide insights to improve Max Life’s marketing strategy
- Reduce marketing costs by targeting the right customers
- Improve customer experience with personalized offers

### **Conclusion**
This project shows how machine learning can help businesses make better decisions. By predicting which customers are interested in health insurance, Max Life can improve sales and customer satisfaction. The insights from this analysis will help the company refine its marketing and offer better services.
