**X Education Lead Scoring Model**

**Project Overview**:

X Education, an online course provider for industry professionals, faces a challenge with a low lead conversion rate of 30%. This project aims to build a predictive model to identify "Hot Leads" and improve the conversion rate to 80%. The model will help the sales team prioritize leads more effectively, leading to better outcomes.

**Goals:**

  1. Build a Logistic Regression model to score leads on a scale of 0-100.
  2. Recommend key strategies based on the model's predictions to enhance conversion rates.

**Dataset:**

The dataset consists of 9000 rows and 15 columns with attributes like:
  1. Lead Source
  2. Total Time Spent on Website
  3. Total Visits
  4. Last Activity The target variable is 'Converted' (1: converted, 0: not converted).

**Lead Source:**
  1. Total Time Spent on Website
  2. Total Visits
  3. Last Activity
  4. The target variable is 'Converted', indicating whether the lead converted (1) or not (0).

**Steps:**
  
  **1. EDA (Exploratory Data Analysis)**
       Remove rows with missing values.
       Perform feature scaling and treat outliers.
       Visualize relationships between features and conversion.
  
  **2. Model Building:**
      Use RFE (Recursive Feature Elimination) to select top 15 features.
      Build a Logistic Regression model and tune using different cutoffs (e.g., 0.35, 0.44).
   
  **3. Model Evaluation:**
      Evaluate the model using ROC AUC, Precision, Recall, and F1 Score to find the best cutoff point.

**Top Features:**
  1. Total Time Spent on Website
  2. Last Activity (SMS Sent)
  3. Total Visits
     
**Recommendations:**
  1. Focus more on sending SMS notifications.
  2. Improve Olark Chat performance, as it's negatively impacting conversion.
  3. Target potential leads with higher website interaction.
     
**Requirements:**
  1. Python 3.x
  2. Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

**How to Run:**
  1. Clone this repository.
  2. Run lead_scoring_model.py to build and evaluate the model.
  3. Adjust cutoff in the script to change focus on leads.

**Conclusion:**
By focusing on "Hot Leads," X Education can achieve higher conversion rates, ultimately improving the sales process and resource utilization. The model can be further enhanced by adding more features or experimenting with other machine learning algorithms.
