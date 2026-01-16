#  Task 3: Predicting Insurance Claim Amounts

##  Overview
This repository contains the solution for **Task 3: Predicting Insurance Claim Amounts**, completed as part of my **AI & Data Science Internship tasks**.  
The task focuses on applying regression techniques to estimate medical insurance costs based on personal and lifestyle-related attributes.

##  Objective
The objective of this task is to predict medical insurance claim amounts using a **Linear Regression model**.  
By analyzing personal data such as age, BMI, and smoking status, we aim to understand how these factors influence insurance charges and evaluate the model’s prediction accuracy.

---

##  Dataset
**Dataset Name:** Medical Cost Personal Dataset  

The dataset contains information about individuals along with their medical insurance charges.

### Features:
- **age** – Age of the individual  
- **sex** – Gender (male / female)  
- **bmi** – Body Mass Index  
- **children** – Number of children covered by insurance  
- **smoker** – Smoking status (yes / no)  
- **region** – Residential region  
- **charges** – Medical insurance cost (**target variable**)

---

##  Tools & Technologies Used
- Python  
- Jupyter Notebook / Google Colab  
- Pandas & NumPy (data handling)  
- Matplotlib & Seaborn (data visualization)  
- Scikit-learn (machine learning & evaluation)

---

##  Approach

### 1️⃣ Data Loading
- The dataset was loaded using **pandas**.
- Initial inspection was done using `.head()` and `.info()`.

### 2️⃣ Data Cleaning & Preparation
- Converted categorical variables into numerical form:
  - `sex` → male = 0, female = 1  
  - `smoker` → no = 0, yes = 1  
- Applied **one-hot encoding** to remaining categorical features.
- Checked for missing values (none found).

### 3️⃣ Exploratory Data Analysis (EDA)
Visualizations were created to understand relationships between features and insurance charges:
- **Age vs Charges** (scatter plot)
- **BMI vs Charges** (scatter plot)
- **Smoking Status vs Charges** (box plot)

### 4️⃣ Model Training
- Selected **Linear Regression** as the prediction model.
- Split the dataset:
  - 80% training data
  - 20% testing data
- Trained the model using the training dataset.

### 5️⃣ Model Evaluation
Model performance was evaluated using:
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**

---

##  Results & Insights

- **Age** has a positive impact on insurance charges.
- **BMI** is directly related to higher medical costs.
- **Smoking status** is the most influential factor in increasing insurance charges.
- The Linear Regression model provides **reasonable predictions** for medical insurance costs.

---

##  Evaluation Metrics
- **MAE**: Shows average prediction error  
- **RMSE**: Penalizes large prediction errors more strongly

 Lower values of both metrics indicate better model performance.

---

##  Conclusion
This task successfully demonstrated the application of **Linear Regression** to predict medical insurance claim amounts.  
By analyzing key personal attributes and evaluating model performance, meaningful insights were gained into factors affecting insurance costs.  
This project serves as a strong foundation for applying more advanced regression techniques in future tasks.  

---

