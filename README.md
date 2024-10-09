# Project Proposal

## Title
**Debunking the Myth: An Analysis of Fine Rates for Custom vs. Standard License Plates in Georgia Using Borbalo Data**

---

### 1. Description of the Project

I developed **Borbalo** in October 2022 as a mobile application to help Georgian drivers stay informed about traffic fines. Borbalo provides real-time notifications of fines, detailed violation histories, and insights into traffic enforcement patterns across different regions. Over the past two years, Borbalo has collected extensive data on traffic fines, including those associated with both custom and standard license plates.

This project aims to investigate the common belief in Georgia that custom license plates are less likely to receive fines compared to standard plates. By analyzing the fine distribution data from Borbalo, I seek to determine whether this myth holds true and to provide evidence-based insights into traffic enforcement practices.

---

### 2. Clear Goals

- **Primary Goal:**  
  To determine if there is a significant difference in the fine rates between custom and standard license plates in Georgia.

- **Secondary Goals:**  
  - Identify factors that contribute to the perception that custom plates receive fewer fines.
  - Assess the fairness and consistency of traffic law enforcement across different license plate types.
  - Provide recommendations to improve public awareness and policy based on the findings.

---

### 3. Data Collection

- **Data Source:**  
  I will export data directly from Borbalo's production database, which records all traffic fines processed through the app.

- **Data to be Collected:**  
  - **License Plate Information:** Type (custom vs. standard), alphanumeric sequences.
  - **Fine Details:** Number of fines issued, types of violations (e.g., speeding, illegal parking), fine amounts.
  - **Vehicle Information:** Make, model, year, vehicle type.
  - **Driver Demographics:** Age, gender (if available and ethically permissible).
  - **Violation Details:** Location (coordinates or designated areas), date and time of each violation.

- **Data Collection Method:**  
  I will use secure SQL queries to export the necessary data from Borbalo's database, ensuring data integrity and compliance with privacy standards. All data will be anonymized to protect individual privacy.

---

### 4. Data Modeling Plan

To analyze the data, I plan to use the following modeling approaches:

- **Descriptive Statistics:**  
  Summarize the distribution of fines across license plate types, including measures like mean and variance.

- **Inferential Statistics:**  
  - **Chi-Square Tests:** To assess the association between license plate type and the occurrence of fines.
  - **T-Tests or Mann-Whitney U Tests:** To compare the average number of fines between custom and standard plates, depending on data distribution.

- **Regression Analysis:**  
  - **Logistic Regression:** To evaluate the probability of receiving a fine based on license plate type while controlling for other variables.
  - **Poisson Regression:** To model the count of fines per vehicle in relation to license plate type and other predictors.

*Note:* I may refine these techniques as I explore the data further during the project.

---

### 5. Data Visualization Plan

To effectively communicate my findings, I plan to use the following visualization methods:

- **Bar Charts:**  
  Compare the total number of fines issued to custom versus standard license plates.

- **Pie Charts:**  
  Show the proportion of different types of violations within each license plate category.

- **Scatter Plots:**  
  Explore relationships between fine amounts and variables such as time of day or location, differentiated by license plate type.

- **Heat Maps:**  
  Visualize the geographic distribution of fines, highlighting areas with higher enforcement rates for each license plate type.

- **Interactive Dashboards:**  
  Potentially use tools like Tableau or Power BI to create dynamic visualizations for deeper data exploration.

---

### 6. Test Plan

To ensure the validity and reliability of my analysis, I will implement the following test plan:

- **Data Splitting:**  
  - **Training Set:** 80% of the data will be used to develop and train the statistical models.
  - **Testing Set:** 20% of the data will be withheld to evaluate model performance.

- **Temporal Validation:**  
  - **Training on Historical Data:**  
    Use data from January 2023 to August 2024 for training.
  - **Testing on Recent Data:**  
    Reserve data from September 2024 to October 2024 for testing to assess the model's generalizability.

- **Cross-Validation:**  
  - **K-Fold Cross-Validation:**  
    Perform 5-fold cross-validation on the training set to evaluate model stability and performance consistency.

- **Performance Metrics:**  
  - **For Classification Models (e.g., Logistic Regression):**  
    Accuracy, Precision, Recall, F1-Score, ROC-AUC.
  - **For Count Models (e.g., Poisson Regression):**  
    Deviance, Akaike Information Criterion (AIC), goodness-of-fit measures.

- **Hypothesis Testing:**  
  - **Null Hypothesis (H₀):** There is no difference in fine rates between custom and standard license plates.
  - **Alternative Hypothesis (H₁):** There is a significant difference in fine rates between custom and standard license plates.
  - Conduct statistical tests to accept or reject these hypotheses based on the data.

- **Assumptions Checking:**  
  Ensure that the assumptions underlying each statistical method are satisfied, such as normality for t-tests or appropriate distributional assumptions for regression models.

*Note:* I may adjust the test plan based on preliminary findings and the specific characteristics of the dataset.

---

### 7. Conclusion

By leveraging the comprehensive data collected through the Borbalo app, this project aims to provide a clear, evidence-based analysis of fine rates associated with custom and standard license plates in Georgia. Through rigorous statistical modeling and thoughtful visualization, I intend to debunk the existing myth and contribute valuable insights to traffic law enforcement practices and public perceptions.

---
