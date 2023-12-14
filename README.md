Group 3
# **Brain Stroke Prediction**
https://www.kaggle.com/code/nerminabdelhafeez/brain-stroke-prediction/notebook

**Disclaimer:** The instructions and code used in the project are based on the provided guidelines

## **Introduction**
A stroke is a dangerous, perhaps fatal medical illness that is caused by an abrupt stoppage of the brain's blood supply. There are two types of strokes: ischemic stroke, that happens when there is a blockage in the blood supply to the brain, and hemorrhagic strokes, which occurs because of abrupt bleeding in the brain.Using input parameters, this project was created to forecast a patient's risk of having a stroke. 

A stroke is a medical emergency. It can result in irreversible brain damage, permanent impairment, or death. The World Health Organization (WHO) reports that stroke ranks as the second most common cause of death worldwide, accounting for around 11% of all fatalities. Fedesoriano's "stroke prediction dataset" – which has 5110 observations with 12 variables – serves as the basis for this project’s dataset. The original dataset has been slightly preprocessed; the "id" columns have been removed, along with a few outliers and highly unusual categorical values. 

Knowing the likelihood of getting a stroke as well as the risk factors may help prevent a stroke now or in the future. A person's chances of suffering damage from a stroke decrease with the time they receive care. The goal of this project is to give those who are at risk of stroke immediate assistance since immediate medical attention is essential.

## **Objectives**
* Conduct descriptive statistics and visualize data distributions.
* Evaluate model performance through metrics such as precision, recall, and accuracy.
* Interpret and compare the outcomes of both Logistic Regression and KNeighbors models.
* Summarize findings and provide insights into the effectiveness of each model for stroke prediction.

## **Methodology**
1. Data Loading:
   > * Import necessary libraries (NumPy, Pandas, Matplotlib, Seaborn).
   > * Load the dataset ('Group 3 - Brain Stroke prediction Dataset.csv') into a Pandas DataFrame.

2. Data Cleaning:
   > * Remove rows with "Unknown" values in the "smoking_status" column.
   > * Check for and handle any null values in the dataset.
   > * Check for and remove duplicate information.

3. Data Transformation:
   > * Convert categorical variables to numerical representations for analysis.

4. Exploratory Data Analysis (EDA):
   > * Generate summary statistics using data.describe().
   > * Check for the distribution of values and count of null values.
   > * Visualize relationships and distributions using various Seaborn plots.
   > * Analyze relationships between variables, such as hypertension, heart disease, and stroke.

5. Data Preprocessing:
   > * Split the data into features (x) and target variable (y).
   > * Further split the dataset into training and testing sets.

6. Logistic Regression:
   > * Implement Logistic Regression model from scikit-learn.
   > * Fit the model to the training data and make predictions on the test data.
   > * Evaluate the model using a classification report, accuracy score, and confusion matrix.

7. KNeighbors Algorithm:
   > * Implement the KNeighbors Classifier from scikit-learn.
   > * Fit the model to the training data and make predictions on the test data.
   > * Evaluate the model using accuracy score and confusion matrix.

8. Results
   > * Analyze and interpret the results from both models, considering accuracy, precision, recall, and the confusion matrix.

## **Result and Discussion**
1. **Gender and Stroke:**
   > ![Screenshot 2023-12-14 145605](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/37ce68d5-137a-42dd-b9b4-a37bd549a8b3)
   > 
   > Figure 1 indicates that the number of females suffering from strokes is higher than the number of males.

2. **Hypertension:**
   > ![Screenshot 2023-12-14 144304](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/a8b38b49-c959-4c27-beea-22dbce922e59)
   > 
   > Figure 2 highlights that a majority of people in the dataset do not have hypertension.

3. **Heart Disease:**
   > ![Screenshot 2023-12-14 144336](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/3b80d94b-866f-4a2b-9cdb-bf88a3c4a369)
   > 
   > Figure 3 shows that most people in the dataset do not have heart disease.

4. **Marital Status:**
   > ![Screenshot 2023-12-14 144407](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/6bd4d7ae-b013-45fb-b5f5-57de9b42665c)
   > 
   > Figure 4 reveals that a significant portion of the dataset consists of individuals who are ever married.

5. **Residence Type:**
   > ![Screenshot 2023-12-14 144439](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/f94e7e74-3af5-4811-9d1d-ff2e180200fc)
   > 
   > Figure 5 suggests that there are more people from urban areas than rural areas in the dataset.

6. **Smoking Status:**
   > ![Screenshot 2023-12-14 144510](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/296d1eed-9e5f-4844-9679-3212ce2637b8)
   > 
   > Figure 6 illustrates that the most common smoking status in the dataset is "never smoked."

7. **Hypertension and Heart Disease Relationship:**
   > ![Screenshot 2023-12-14 144606](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/3f235ed8-1635-4d5c-a40b-4f7f31b25202)
   > 
   > Figure 7 indicates there is no clear relationship between hypertension and heart disease.

8. **Smoking Status by Gender:**
   > ![Screenshot 2023-12-14 150233](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/034ce8a6-bbf6-4163-9ac3-887d7c32f272)
   > 
   > Figure 8 presents the smoking status distribution between male and female.

9. **Model Accuracy:**
    > The logistic regression model achieved an accuracy of 94%. The K-nearest neighbor model achieved an accuracy of 93%.

    **Logistic Regression Model**
   ![Screenshot 2023-12-14 145920](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/4c482507-a792-4ea8-828c-06c3a369cde2)
   ![Screenshot 2023-12-14 150028](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/f6073d16-ee58-485a-ab44-eb436e23f881)

    **K-nearest Neighbor Model**
   ![Screenshot 2023-12-14 150119](https://github.com/xrjac/Group-3-Final-Project/assets/149233085/e0c6c318-5eed-482f-8353-984fc960a6f8)


### **Observations:**

The analysis of the dataset reveals several noteworthy trends. Firstly, there is a notable gender-specific pattern in stroke prevalence, with a higher number of females suffering from strokes compared to males (Figure 1). The dataset predominantly comprises individuals without hypertension (Figure 2) or heart disease (Figure 3), suggesting a generally healthy population. The prevalence of individuals who are ever married (Figure 4) hints at a demographic skew towards older or more traditionally married individuals. Moreover, the dataset is skewed towards urban residents (Figure 5), possibly reflecting either the sampling method or a genuine demographic trend. The majority of individuals in the dataset are non-smokers (Figure 6), indicating positive health behavior. Interestingly, there appears to be no clear relationship between hypertension and heart disease (Figure 7), suggesting these conditions may be relatively independent in the dataset. The examination of smoking patterns by gender (Figure 8) may provide insights into gender-specific health behaviors. Notably, both the logistic regression and K-nearest neighbor models exhibit high accuracy (94% and 93%, respectively), indicating their effectiveness in predicting or classifying health-related outcomes within the dataset. While these findings offer valuable insights, it's important to emphasize that they are based on observational data, and further research is needed to establish causation or generalize the findings to broader populations.

## **Conclusion**
This analysis holds several aspects of the population's health and background, aligning with the project's goals of deciphering health trends and forecasting potential outcomes. We observed a higher stroke prevalence in females, a predominantly healthy population with low hypertension and heart disease rates, and a skew towards married, urban residents who have never smoked. Intriguingly, the data offered no clear link between hypertension and heart disease, suggesting the potential independence of these conditions within this specific population. The high accuracy of the logistic regression and K-nearest neighbor models indicate their potential for predicting health outcomes. 

These findings contain practical implications for healthcare. The observed gender disparity in stroke prevalence warrants further investigation into potential risk factors and targeted preventive measures for women. The low prevalence of hypertension and heart disease suggests a generally healthy population, but further research is needed to understand the factors contributing to this trend. Demographic characteristics, such as marital status and residence type, can inform healthcare resource allocation and patient outreach strategies. However, it's crucial to acknowledge the inherent limitations of observational data, as it precludes drawing causal conclusions and may not readily translate to broader populations. The potential biases in the sampling process or data collection could affect the observed trends in future research that should address these limitations by employing robust methodologies and exploring diverse populations to gain more comprehensive insights.

Furthermore, the analysis offers valuable knowledge about the population's health and a foundation for further research with healthcare professionals and researchers that develop targeted interventions and improve healthcare delivery for specific populations.
