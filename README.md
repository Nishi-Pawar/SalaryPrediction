# SalaryPrediction

📌 Project Overview
This project predicts salaries from job postings by analyzing various features such as job title, company details, and location. Using data scraped from Glassdoor, the project cleans raw salary ranges, engineers meaningful features, and applies machine learning models to estimate average salaries.

📂 Dataset
Source: Glassdoor job listings dataset (glassdoor_jobs.csv)
Key Features:
Job Title
Rating
Size
Type of Ownership
Industry
Sector
Revenue
Location
Derived features: Average Salary, Company Age

⚙️ Data Preprocessing
Parsed raw salary strings (e.g., $70K-$90K) into numerical values.
Computed Average Salary for each job.
Engineered Company Age feature from founding year.
Removed null and inconsistent entries.
Encoded categorical variables using OneHotEncoder.
Split data into training and testing sets.

🤖 Models Used
Ridge Regression
XGBoost Regressor
Additional experiments with pipelines for preprocessing + modeling.

📊 Evaluation
Metrics: Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), R²
Compared model performances to choose the best predictor.
Ridge and XGBoost achieved competitive results for salary prediction.
