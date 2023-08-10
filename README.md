# CVD-Project

## Introduction
Cardiovascular disease (CVD) presents a significant public health challenge, impacting millions of people worldwide (World Health Organization [WHO], 2019). It is known to be the leading cause of global mortality, resulting in over 17 million deaths annually. Early detection of CVD is critical in reducing morbidity and mortality rates. Timely and effective treatment can prevent or slow disease progression. Conventional diagnostic methods for CVD, such as physical examinations and diagnostic tests, are often time-consuming, resource-intensive, and prone to errors.

This project explores the potential of machine learning algorithms for CVD diagnosis. These computational techniques enable computers to learn from data and make predictions. In recent years, machine learning has gained significant attention in medical research, showing promising results in various medical fields, including CVD diagnosis. By training machine learning algorithms on a vast dataset of patient information, such as demographics, lifestyle factors, and medical history, patterns can be identified, and predictions about the likelihood of a patient having CVD can be made.

This project takes up two clients:
  The Nairobi West Hospital who are interested in the potential of machine learning algorithms to enhance CVD diagnosis accuracy.
  Patients for whom the potential machine learning algorithm will improve the efficiency of diagnosis and treatment leading to improved patient care and outcomes.

## Business Understanding
Our goal is to leverage machine learning algorithms to improve the diagnosis of cardiovascular disease (CVD) at Nairobi West Hospital. By employing advanced techniques, we aim to provide healthcare professionals with more accurate insights, enhancing diagnostic accuracy and patient care. This project involves a careful review of current research and an evaluation of various machine learning algorithms to determine their effectiveness in CVD diagnosis. Our approach aligns with the hospital's commitment to innovation and excellence in patient care, and it represents a strategic investment in cutting-edge medical technology. The successful implementation of this project will not only benefit the hospital but also the broader community seeking advanced and precise medical care for CVD.

## Metric of success 
An accuracy of above 80% was chosen as a metric of success to assess prediction accuracy.

## Problem Statement 

The Nairobi West Hospital is in search of a more streamlined and dependable approach of diagnosing CVD and aims to provide patients with expedited diagnostics and mitigate the potential for adverse
outcomes.

## Objectives
Effective Communication of Insight
  Summarize research findings in a clear and concise manner that aligns with the data-driven initiatives of the Nairobi West Hospital.
Development and Application of a Predictive Model
  Apply machine learning algorithms to build a predictive model that accurately assesses the risk level of patients for developing cardiovascular diseases.
  Optimize model parameters to ensure high diagnostic precision and minimize false positives and false negatives.

## Data Understanding 

The Cardiovascular Diseases Risk Prediction Dataset was sourced from Kaggle. This dataset includes 308854 rows x 19 columns. The columns in this dataset include the following:

General Health: This is a measure of the degree of health of the patient which ranges from poor to excellent.
Checkup: This is how long it has been since the patient's last checkup.
Exercise: A column of yes and no of whether the patient has participated in exercise during the past month.
Skin_Cancer: Whether or not a patient has skin cancer.
Other_Cancer: Whether or not a patient has other cancers apart from skin cancer.
Depression: Whether or not a patient has depression or not.
Diabetes: Whether or not a patient has Diabetes.
Arthritis: Whether or not a patient has Arthritis.
Sex: The gender of a patient be it male or female.
Age_category: The range of ages in which a patient falls into be it 60-64, 75-79 or even 80+ years
Height: The height of a patient in centimeters.
Weight: The weight of a patient in kilograms.
BMI: The ratio of the height of a patient to his/her weight which shows whether a patient is under or overweight.
Smoking_history: Whether or not a patient is a smoker or not.
Alcohol_Consumption: The level of alcohol consumption of a patient.
Fruit_Consumption: The level of fruit consumption of a patient.
Green_Vegetables_Consumption: The level of green vegetable consumption of the patient.
FriedPotato_Consumption: The level of fried potato consumption of the patient.

## Exploratory Data Analysis 
## 1) Numerical_features                                                                                                                                    
We did univariate analysis on the numerical features to check the distribution of numerical features and these were our findings;                                 
a) Distribution of height follows a normal distribution                                                                                                             
b) Distribution of weight follows a normal distribution                                                                                                             c) Distribution of BMI follows a normal distribution                                                                                                                                                                                                                          
d) Distribution of fruit consumption shows a right-skewed distribution                                                                                              
                                                                                                                                                                   e) Distribution of alcohol consumption shows a right-skewed distribution                                                                                            f) Distribution of green vegetable consumption shows a right-skewed distribution                                                                                    
                                                                                                                                                                    g) Distribution of fried potato consumption shows a right-skewed distribution                                                                                      

## 2) Categorical Features                                                                                                                         
We did an analysis of the distribution of categorical features in the dataset and these were our findings;                                                   
a) The count of the general health of patients shows that the category of patients in very good health is the most by count, followed by the ones in good health and the least represented by count are the ones in poor health.                                                                                                     
                                                                                                                                                                  b) The count of patients who go for a checkup reveals that the category with the largest count was the category of patients who went for a checkup within the past year, followed by the ones that went within the past 2 years and the least by count were the ones that had never gone for a checkup.                                
                                                                                                                                                                    c) The count of patients who exercise is much higher than the ones who do not.                                                                                                                                                                                                                                                        d) The count of patients who do not have heart disease is much higher than those patients with heart disease.                                                       e) The count of patients with depression is a fourth of the ones without depression                                                                                 
                                                                                                                                                                  f) The count of patients with no skin cancer is greater than the ones with cancer. The same findings apply to the count of patients with other types of cancer.     g) The count of patients with no diabetes is the highest count while the count of female patients with diabetes only during pregnancy has the least count.          
                                                                                                                                                                  h) The count of patients with arthritis is half the count of the people without diabetes.                                                                           
                                                                                                                                                                  i) The count of patients who do not smoke is only slightly higher than those patients that do not smoke.                                                           

## 3) Bivariate Analysis                                                                                                                              
We performed bivariate analysis to analyze the relationship between heart condition and some selected variables and these were our findings;                  
a) The relationship between general health and heart disease - we observed that the patients in excellent health showed a very little count of heart disease, while the patients in very good health showed a very high count of no heart disease while the patients in poor health showed that about half of those had heart disease.  b) The relationship between exercise and heart disease - we observed that the patients who exercised more frequently recorded a high count of patients with no heart disease.                                                                                                                       
c) The relationship between sex and heart disease - we observed that the patients who were male had a higher count of patients with heart disease than the patients who were female.                                                                                                                                                   d) The relationship between age category and heart disease - we observed that the patients who were 80 years and older showed the highest prevalence to heart disease.                                                                                                                                                 
e) The relationship between smoking history and heart disease - we observed that the patients who did not smoke recorded a lower count of heart disease compared to the patients who did smoke.    

## Modelling 


## Conclusions 
- The number of heart disease cases increases with age category. 'Older' people tend to be affected more by heart disease compared to young people.

- There is little difference between the male and female category. Although both genders are susceptible to heart disease, the male gender is more affected.

- Based on 'BMI Category', underweight people are less likely to be affected by heart disease while overweight and obese people are more likely to have heart diseases. It is important to note is that normal-weight people are still susceptible to heart disease even if not as much as the others.

- The best model was KNN, with an accuracy of 94% after hyperparameter tuning. However, it was too computationally expensive as it took more than 6 hrs to return results.    
- Our selected model is therefore the decision tree which gave an accuracy of 90.78%. 
This accuracy conveys that the model will give the right predictions over 90% of the time.

## Recommendations 
- With an accuracy of above 90%, we recommend that health practitioners use the decision tree algorithm generated in this project as the first screening for suspected heart disease cases. 

- We recommend that patients maintain good overall health through healthy habits and regular check-in in order to lower the risk of heart disease.

- Patients who are 55 and older are advised to attend regular screenings to aid in the early detection and management of heart conditions.

- It is recommended that the Nairobi West Hospital promote smoking cessation programs and continue to raise awareness about the cardiovascular risks associated with smoking.

