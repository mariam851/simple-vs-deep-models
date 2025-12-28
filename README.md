# Simple vs Deep Models: Course Completion Prediction

## Overview
This project explores the performance difference between simple models (like Logistic Regression) and deep learning models on tabular data. Using a "Course Completion" dataset, we evaluate whether complex deep models outperform simple baselines.

## Dataset
The dataset contains information about students and their interaction with online courses:
- **Categorical features:** Gender, Education_Level, Employment_Status, City, Device_Type, Payment_Mode, etc.
- **Numerical features:** Age, Instructor_Rating, Login_Frequency, Average_Session_Duration_Min, Video_Completion_Rate, etc.
- **Target:** Completed (Yes/No)

## Approach
1. **Data preprocessing**: Encoding categorical variables, scaling numerical features.
2. **Baseline model**: Logistic Regression
3. **Deep model**: Fastai Tabular Learner with embeddings for categorical variables
4. **Evaluation metrics**: Accuracy, ROC-AUC, Confusion Matrix

## Results
- **Logistic Regression:** Accuracy = 59.7%
- **Deep Tabular Model:** Accuracy = 58.8%
- Deep model showed overfitting despite high complexity; simple models performed similarly or better.

## Insights
- Tabular datasets may have low signal-to-noise ratio
- Feature selection and careful preprocessing can be more effective than adding deep layers
- Start simple → then move to complex models (fast.ai philosophy)

## How to run
1. Clone the repository
2. Install required packages: `pip install -r requirements.txt`
3. Run the notebook: `Course_Completion_Analysis.ipynb`

## Author
Mariam Ali
