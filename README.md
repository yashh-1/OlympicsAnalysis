# 🏅 Olympics Medal Analysis (1976–2008)

This project analyzes historical Olympic medal data to uncover trends across countries, genders, and sports.  
It uses exploratory data analysis (EDA), feature engineering, and machine learning to understand and predict medal outcomes.

---

##  Dataset Overview

- **Data Range**: 1976 – 2008 (Summer Olympics only)  
- **Source**: Historical Olympic records  
- **Key Columns**:
  - `Year`, `Country`, `Gender`, `Sport`, `Event`, `Medal`
  - Derived: `Country_Year_Medals`

---

##  Project Workflow

###  Step 1: Data Cleaning
- Handled missing/null values
- Verified data types and formats
- Removed duplicates and inconsistencies
- Encoded categorical variables using LabelEncoder

###  Step 2: Exploratory Data Analysis (EDA)
- Gender-wise medal count heatmap  
- Correlation heatmap of numerical features  
- Country-wise and sport-wise medal distribution  
- Medal trends by year  
- Feature importance for medal prediction

###  Step 3: Machine Learning
- **Model**: Random Forest Classifier  
- **Target**: `Medal` (Encoded: Gold, Silver, Bronze)  
- **Features**: 
  - `Year`, `Gender`, `Country`, `Sport`, `Event`, `Country_Year_Medals`  
- **Evaluation**:
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1 Score)
- **Saved Model**: `olympics_medal_predictor_model.pkl`

###  Step 4: Key Insights
- Certain countries and sports consistently dominate medal counts  
- Gender participation has grown steadily across Olympics  
- `Country`, `Sport`, and `Event` are top predictors for medal type  
- Heatmaps and barplots revealed performance and diversity trends

---

##  Tools & Libraries

- python (Pandas, Matplotlib, Seaborn, Scikit-learn, Plotly)
- Jupyter Notebook
- Joblib (for model saving)
- LabelEncoder & RandomForestClassifier (for ML)

---

