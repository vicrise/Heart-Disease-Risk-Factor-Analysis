# Heart Disease Risk Factor Analysis
### PROJECT OVERVIEW
This project aims to analyze heart disease risk factors using a dataset of 500 patients, The goal is to identify patterns and potential risk factors associated with heart disease, providing valuable insights for prevention and diagnosis.
### PROBLEM STATEMENT 
Heart disease is a leading global cause of death. Traditional diagnostic methods rely on known risk factors like blood pressure, cholesterol, and heart rate, but their impact varies.
The problem this project addresses are which factors significantly contribute to heart disease, are there clear patterns in patient demographics (e.g., age, gender differences), how do Blood Pressure, Cholesterol, and Heart Rate relate to heart disease
### OBJECTIVES
1.	To compare patients with and without heart disease
2.	To analyze how heart disease prevalence changes across different age groups
3.	To investigate whether males or females are more prone to heart disease
4.	To categorize BP levels (Normal, Elevated, Hypertension Stages 1 & 2) and analyse their impact on heart disease.
5.	To classify cholesterol levels (Normal, Borderline, High) and evaluate their relationship with heart disease
6.	To determine whether low, normal, or high heart rates are linked to an increased risk of heart disease.
### DATA SOURCE 
Kaggle 
### METHODOLOGY
#### TOOL USED: Power Query and Power BI
#### DATA CLEANING PROCESS AND TRANSFORMATION: 
- By using a conditional column, I added three additional columns to the dataset, namely the Blood Pressure category that categorizes the blood pressure column into healthy (<120), elevated (120-129), hypertension stage 1 (130-139) and hypertension stage 2 (140 and higher) 
- Cholesterol Category, which categorises the cholesterol column into normal (<200), borderline (200-239) and high (>240)
- Heart rate categories: The heart rate column is divided into normal (60-100) and fast (>100)
### DAX FUNCTION 
-	TOTAL PATIENTS = COUNT('Heart Prediction  Dataset'[Age]) 
-	AVERAGE AGE = ROUNDUP(AVERAGE('Heart Prediction  Dataset'[Age]),0)
-	AVERAGE BLOODPRESSURE = ROUNDUP(AVERAGE('Heart Prediction  Dataset'[BloodPressure]),0)
-	AVERAGE CHOLESTEROL = ROUNDUP(AVERAGE('Heart Prediction  Dataset'[Cholesterol]),0)
-	AVERAGE HEARTRATE LEVEL = ROUNDUP(AVERAGE('Heart Prediction  Dataset'[HeartRate]),0)
### DATA ANALYSIS
- Identify patterns and potential risk factors associated with heart disease, using cholesterol level, blood pressure and heart rate level, providing valuable insights for prevention and diagnosis
- Demographic analysis of age and gender prevalence to heart disease
### KEY INSIGHTS AND RECOMMENDATION
![Screenshot (126)](https://github.com/user-attachments/assets/8f4dc50b-73c5-4f6d-a85d-a22940654908)

- 40% (200 out of 500) of patients have heart disease, while 60% (300) do not. This indicates a significant prevalence of heart disease among the studied population.
  
![Screenshot (123)](https://github.com/user-attachments/assets/2ec5b566-cceb-47d7-a50f-7a9ff30107a7)

#### INSIGHT
- 114 patients with hypertension stage 2 have heart disease, compared to 100 without. This suggests that severe hypertension is a strong risk factor for heart disease.  
- Surprisingly, 122 patients with normal blood pressure have heart disease, which is more than those without (59). This indicates that other factors (e.g., cholesterol, heart rate, lifestyle, and genetics) contribute to heart disease risk, even when blood pressure.  
- 42 patients with elevated blood pressure have heart disease, while only 19 do not. This suggests that even slightly increased blood pressure can be a risk factor.  
- Patients in the hypertension stage 1 category are equally divided (22 with heart disease, 22 without). This suggests that early-stage hypertension alone may not be a strong predictor but could lead to heart disease if combined with other risk factors.  
#### RECOMMENDATION
- Encourage regular monitoring, medication adherence, low-sodium diets, exercise, and stress management for Hypertension Stage 2 Patients. 
- Since many patients with normal blood pressure still have heart disease, cholesterol levels, heart rate, obesity, diabetes, smoking, and family history should be examined. A multifactorial risk assessment should be implemented to identify other contributors.   
- Since elevated blood pressure already shows a significant heart disease association, preventive measures like lifestyle modifications (diet, weight management, exercise) should be encouraged before it progresses to hypertension.  
- Even though the split is equal, patients in stage 1 hypertension should be monitored for worsening conditions.  
- Lifestyle changes and mild medical interventions may help prevent progression to stage 2. 
- Patients should not only focus on blood pressure control but also manage cholesterol, physical activity, and diet to reduce overall cardiovascular risk.  
- Encourage regular screenings and early detection for those at risk.  

![Screenshot (124)](https://github.com/user-attachments/assets/42f93ef6-7d17-446f-ab4c-cbb0669b41e5)

#### INSIGHT
- Among patients with a normal heart rate, 205 have heart disease, while 128 do not. This suggests that a normal heart rate does not guarantee protection from heart disease.  
- Among patients with a Fast heart rate, 95 have heart disease, while 72 do not. A higher heart rate may indicate underlying cardiovascular stress or conditions such as Arrhythmia, hypertension, or metabolic issues.  
- Since both normal and fast heart rate categories have a high number of heart disease cases, this suggests that heart disease is influenced by multiple factors beyond just heart rate, such as blood pressure, cholesterol, and lifestyle. 
#### RECOMMENDATION 
- Since many heart disease patients have a normal heart rate, clinicians should not rely on heart rate alone as an indicator of heart disease risk.  
- Regular checkups, including ECG, cholesterol levels, blood pressure, and lifestyle assessments, should be conducted.  
- Since patients with fast heart rates also have a significant heart disease presence, they should be monitored for arrhythmia, hypertension, and autonomic dysfunction.  
- Lifestyle modifications such as stress management, hydration, and exercise regulation should be encouraged.

![Screenshot (125)](https://github.com/user-attachments/assets/6ae43ebc-5332-4c9a-871b-056cd205080d)

#### INSIGHTS 
- 150 patients with normal cholesterol levels have heart disease, compared to only 35 without heart disease. This suggests that heart disease is not solely dependent on high cholesterol and may be influenced by other factors like blood pressure, heart rate, lifestyle, and genetics.  
- Among patients with high cholesterol, 124 do not have heart disease, while only 67 do. This challenges the common assumption that high cholesterol directly leads to heart disease in all cases. Some individuals with high cholesterol might have protective factors such as a healthy diet, active lifestyle, or effective medication use.
- Among patients with borderline cholesterol, 83 have heart disease, compared to 41 without heart disease. This suggests that even moderately high cholesterol levels require monitoring and early intervention to prevent heart disease progression.  
#### RECOMMENDATION
- Since heart disease is highest in those with normal cholesterol, clinicians should assess other risk factors, including blood pressure, BMI, smoking habits, and stress levels.  
- Conduct regular cardiovascular screenings instead of relying solely on cholesterol as an indicator of heart disease risk.  
- Patients with borderline or high cholesterol should adopt a heart-healthy diet (low in saturated fats, rich in fiber and healthy fats), regular exercise, and stress management.  
- Consider evaluating LDL vs. HDL cholesterol levels, inflammatory markers (like C-reactive protein), and genetic predisposition*to determine true risk.  
- Since heart disease cases are significant in the borderline cholesterol category, patients should be monitored closely and advised on preventive measures before they progress to a high-risk category.
   
### CONCLUSION 
- Heart disease is multifactorial and cannot be predicted based on a single parameter like blood pressure, heart rate, or cholesterol alone.
- Patients with normal cholesterol or blood pressure should not be overlooked—other risk factors such as lifestyle, genetics, and stress play a role.
- Preventive measures, such as regular screenings, lifestyle modifications, and personalized treatment plans, are essential to managing heart disease risks.

- [INTERACTIVE DASHBOARD](https://app.powerbi.com/groups/me/reports/4915fba7-ffca-40a0-868b-1dab603c1005/2c96688b224ec6ea3d28?experience=power-bi)


