# 2024_ia651_Ramesh_Suryadevara
# Polycystic Ovary Syndrome Without Fertility Issues
## Table of Contents
- [Introduction](#Introduction)
- [Objective](#Objective)
- [Dataset](#Dataset)
- [Methodology](#Methodology)
- [Explorartory Data Analysis](#Explorartory_Data_Analysis)
- [Machine learning techniques used](#Machine_learning_techniques_used)
- [Interpretation](#Interpretation)
- [Conclusion](#Conclusion)

## Introduction
Polycystic Ovary Syndrome (PCOS) is a prevalent endocrine disorder impacting women of reproductive age worldwide. Characterized by a spectrum of symptoms including irregular menstrual cycles, obesity, insulin resistance, and hyperandrogenism, PCOS significantly affects a woman's quality of life and poses long-term health risks. The disorder's etiology is complex, involving an interplay of genetic, environmental, and lifestyle factors, which contribute to its heterogeneity and the variability in its manifestation.

##  Objective
The primary objective of this research is to conduct a comprehensive analysis of a dataset containing health and lifestyle variables from a diverse group of women, aiming to identify patterns and associations that may influence the presence and severity of PCOS. Through the application of advanced statistical and data mining techniques, this study seeks to unravel the multifactorial interactions that contribute to PCOS, aiming to pinpoint key predictors that could aid in early identification and personalized treatment strategies.Furthermore, the study endeavors to enhance the understanding of PCOS beyond the common perspective of fertility issues, providing insights that could lead to more effective management and treatment approaches for all manifestations of the syndrome.

## Dataset
The data set is collected from Kaggle [\[PCOS\]](https://www.kaggle.com/prasoonkottarathil/polycystic-ovary-syndrome-pcos) from 10 different hospitals across Kerala, India in the year 2020. 

### Features
This dataset includes 541 observation with a total of 46 variables:

  For Yes/ No variables Yes= 1 and No = 0.
![image](https://github.com/user-attachments/assets/f62c4933-b741-4e1a-9803-07ffd1d1b252)

1. RR(breaths/min): Respiration rates.
2. Hb(g/dl): Hemoglobin levels that measures how much hemoglobin is in your blood.
3. Cycle(R/I): 4 indicates irregular menstrual Cycle.
	            2 indicates regular menstrual Cycle.
4. Beta-HCG: Mentioned as two cases I and II (These are pregnancy hormones). The detection of beta hCG (I) shows more accuracy in pregnancy test than in beta hCG (II) .
5. FSH- Follicle stimulating Hormone.
6. LH- luteinizing hormone.
7. TSH - thyroid stimulating hormone.
8. PRL-  prolactin in blood
9. RBS means Random glucose test
10. PRG means PCOS related genes
11. BMI- Body Mass Index.

### Target Variable
The target variable is **PCOS (Y/N)** which has Yes and No variable.

### Data Preprocessing 
The dataset which includes various health parameters a standard data preprocessing pipeline would involve several steps to ensure the data is clean, relevant, and structured in a way that can be effectively used for analysis or modeling. We first handled the missing values by removing rows or columns with a high percentage of missing data. Use statistical tests to determine the significance of variables with respect to the outcome variable (PCOS in this case) and remove non-significant features.

## Methodology
![image](https://github.com/user-attachments/assets/6329f118-de59-4c53-b2b7-bcf5553f944b)

## Explorartoy Data Analysis
1. ### Correlation Matrix
 We have used heat map as it allows you to visually inspect the relationships between variables, which are quantified using Pearson correlation coefficients. Factors such as 'BMI', 'Weight (Kg)','Marraige Status (Yrs)', 'Age (yrs)', 'Waist (inch)', 'Hip(inch)','Follicle No. (R)', 'Follicle No. (L)' have a strong correlation with the target variable.
![image](https://github.com/user-attachments/assets/7d5c6851-0026-4744-bb47-adcddd3bfd4e)

2. ### Box Plots
   #### For Non Binary Features 
   ![image](https://github.com/user-attachments/assets/c4f9823c-9d16-47a7-824e-2dfd68c7c198)
   ![image](https://github.com/user-attachments/assets/22348347-1ffc-4852-b890-5822046687ac)
   ![image](https://github.com/user-attachments/assets/fbcb7a12-2b4c-48ac-9ced-a023d39d53ba)
   ![image](https://github.com/user-attachments/assets/783d8caf-7741-4db6-93ff-a550ee7b815d)
   ![image](https://github.com/user-attachments/assets/30b62052-6b1a-4f06-8000-f6b8a63d2760)
   ![image](https://github.com/user-attachments/assets/5f5b233e-c225-472e-9e70-08f3948dbc9a)
   ![image](https://github.com/user-attachments/assets/a290fd77-6068-4200-af85-ea02fc99e819)
   ![image](https://github.com/user-attachments/assets/2b91431b-970f-4834-8807-1d3d5b818380)
   ![image](https://github.com/user-attachments/assets/eb6fe61c-389e-4172-a249-6ec3526b1505)
   ![image](https://github.com/user-attachments/assets/89548701-48e1-48c5-a1d2-ce811767e122)
   ![image](https://github.com/user-attachments/assets/936493b9-187d-4ca0-8afa-2e88b47e9ad4)
   ![image](https://github.com/user-attachments/assets/e8c2435a-6773-4408-9317-f22a2e4af541)

3. ## Bar Graphs
   ### For Binary Features
   ![image](https://github.com/user-attachments/assets/31a98fad-9a67-447c-b809-e5844b5ce4d6)
   ![image](https://github.com/user-attachments/assets/a676076a-9ec7-414b-a528-275dc9787521)
   ![image](https://github.com/user-attachments/assets/ec69d549-8c86-4fd8-bc60-f8b93d00a5a3)
   ![image](https://github.com/user-attachments/assets/950f097c-e546-4e74-9faf-bbe95941e763)
   ![image](https://github.com/user-attachments/assets/29ba67c6-1195-43bf-a289-eddfe4b0fc29)
   ![image](https://github.com/user-attachments/assets/7608ccc2-8c3b-4445-b387-cc83c267b91c)
   ![image](https://github.com/user-attachments/assets/5f954105-0ce2-4956-80f2-eb1c900438a2)
   ![image](https://github.com/user-attachments/assets/eecf44ea-6959-47e3-85a5-e0197e104fcf)
   ![image](https://github.com/user-attachments/assets/a1f3049f-652f-4b38-9e5f-7577f633ed90)

4. ## Scatter Plots
   ![image](https://github.com/user-attachments/assets/c2dd5035-98d3-4e25-ac83-ff052c458400)
   ![image](https://github.com/user-attachments/assets/2ed05bc9-b8cd-41c7-b85c-77e874b9c216)
   ![image](https://github.com/user-attachments/assets/aea4d883-95b1-4507-a28f-4665e2c03067)

## Machine Learning Techniques Used
We used a few machine learning techniques to know which feature is affecting to be diagnosed with PCOS.

1. Logistic Regression
2. Lasso Regression
3. Random Forest Classifier.

## Interpretation 
The above mentioned models were used on the dataset and we got the following:

  ### Accuracies
  - Average Logistic Regression Accuracy : 0.8466257668711656
  - Average Lasso Regression Accuracy : 0.8159509202453987
  - Average Random Forest Classifier : 0.901840490797546

### Logistic Regression- Feature Scores
This chart represents the feature scores from logistic regression analysis. Each bar represents a feature from the dataset, and the length of the bar indicates the magnitude of the feature's coefficient in the logistic regression model.
     - Follicle No.(R), Cycle(R/I), BMI, Skin Darkening(Y/N), Hair Growth(Y/N) have the highest positive score, indicating it is a strong predictor of PCOS.
![image](https://github.com/user-attachments/assets/2f098de4-dc4b-4782-8dc5-df47df1c50f5)

### Lasso Regression- Feature Importance
This chart givs feature importance as determined by a Lasso regression analysis, which is a type of linear regression that includes a regularization parameter to prevent overfitting and help in feature selection by shrinking some coefficients to zero. 
- Follicle No.(R) continues to show the highest importance, similar to the previous logistic regression analysis.
- Height(cm) and BMI these features are highly important in this model, there is a significant association between a woman's body mass index and height with the occurrence of PCOS.
![image](https://github.com/user-attachments/assets/2262e091-85aa-48ad-8cf5-3b9acce8c96e)

### Random Forest Classifier - Feature Scores
Each feature is useful at predicting the target variable, in this case, likely the presence or severity of Polycystic Ovary Syndrome (PCOS).The model's emphasis on different features compared to other models like Lasso or Logistic Regression underscores the complex nature of PCOS, where multiple factors interact in complex ways, and different models may capture these interactions differently.  
![image](https://github.com/user-attachments/assets/e60f09d3-063e-4bd4-a48a-a20879c30d67)

## Conclusion

The analysis across various machine learning models—Logistic Regression, Lasso Regression, and Random Forest Classifier—provides a comprehensive understanding of the factors influencing Polycystic Ovary Syndrome (PCOS). Each model, through its unique approach and interpretation of the dataset, highlights important predictors and their relationships with the presence and severity of PCOS. 
### Key Conclusions
1. Physiological Factors are Paramount:
      - Folllicle No.(R) is continues to show the highest importance for all the models.
      - Age and Weight: Consistently, age and weight emerge as top predictors across all models, underlining the influence of demographic and physiological factors on PCOS.
      - BMI and Height: These factors also rank highly, emphasizing the role of body composition in PCOS. The direct correlation between obesity and PCOS is well-established, and the models 
        reinforce this connection.

2. Reproductive and Hormonal Indicators:
      - Menstrual Cycle Regularity: The regularity and length of menstrual cycles are significant predictors, directly linking to reproductive health and PCOS symptoms.
      - Follicle Count: Particularly the number of follicles in the right ovary, highlighted in several models, underscores its importance as a biological marker in diagnosing PCOS.

In conclusion, the findings from these machine learning models offer valuable insights into the complex etiology of PCOS, highlighting key areas for clinical focus and research exploration. By integrating these insights, healthcare providers can enhance diagnostic accuracy and tailor interventions that are more effective in managing and potentially alleviating the burden of PCOS.





   










































