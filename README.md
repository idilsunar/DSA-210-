# Effects of Sleep Patterns on the Life Quality Of College Students

## 1. Project Overview
This project investigates the relationship between sleep patterns and the life quality of university students. It aims to assess how sleep duration and quality correlate with well-being indicators such as caffeine intake, screen time, physical activity and stress levels.The data will be gathered from a self-reported survey and enriched using public datasets, then the data will be analyzed using exploratory and statistical methods.

I will test the validity of the following hypothesis:

Null Hypothesis (H₀): There is no significant relationship between sleep patterns and well-being indicators among university students.

Alternative Hypothesis (H₁): There is a significant relationship between sleep patterns and well-being indicators among university students.

| Well-being Variables     | Sleep Variables                    |
|--------------------------|------------------------------------|
| Stress Level             | Sleep Duration                     |         
| Screen Time              | Sleep Quality                      |
| Caffeine Intake          | Sleep Quality                      |
| Physical Activity Level  | Sleep Quality                      |


## 2. Motivation
I noticed that university students often suffer from irregular sleep schedules and high stress, especially during midterm weeks and finals. Understanding how sleep affects well-being can help students adopt healthier habits and improve academic performance and their quality of life. Furthermore, I plan to better understand the data science concepts that we have learned during DSA210 by applying these concepts into daily life situations that concern many students such as myself.

## 3. Data Sources

I will retrive data from the following:

### 3.1. Custom Survey
A Google Form was created and shared among university students to gather first-hand data. The survey includes questions about:

* *   Sleep duration
* *   Bedtime and wake-up times
* *   Self-reported stress, anxiety, focus, and efficiency levels -Link:
  *   https://docs.google.com/forms/d/e/1FAIpQLSfzbsUjo9XQQTqDkXibk7uiqshNAtH5bJ6ntHw5EUVsY9YSXg/viewform?usp=header)
    
    
### 3.2. Public Datasets:
* *   [Kaggle - Student Sleep Patterns](https://www.kaggle.com/datasets/arsalanjamal002/student-sleep-patterns?resource=download)
* *   [Kaggle- SleepQual and B.Health dataset](https://www.kaggle.com/datasets/anshika1011/sleepqual-and-bhealth-dataset)

### 4. Data Analysis Plan  
- **Exploratory Analysis**  
  - Analyze sleep duration, consistency, bedtime vs wake-up patterns.  
- **Hypothesis Testing**  
  - Use ANOVA and correlation tests to assess links between sleep and well-being scores.  
- **Visualization**  
  - Bar plots, heatmaps, and scatter plots to illustrate relationships.  
- **Modeling**  
  - **Logistic Regression** (baseline)  
  - **Random Forest** (tuned via RandomizedSearchCV)  
  - **Gradient Boosting** (tuned via RandomizedSearchCV)  
  - **Hyperparameter tuning** for all models using 5-fold cross-validation and ROC AUC as the scoring metric  


## 4.1 Data Enrichment Strategy
To strengthen the analysis, the self-reported survey data collected from university peers is enriched with multiple publicly available datasets. These external sources provide additional variables such as wearable-tracked sleep quality, biometric data, and mental health indicators collected in different contexts. By combining local and public datasets:

* *   I will enhance the variety and richness of features available
* *   I will increase the overall sample size for more robust analysis
* *   And we will have a comparison between self-reported and sensor-based sleep metrics

## 5. Tools and Technologies
* *   **Language**: Python
* *   **Libraries**: Pandas, NumPy, Seaborn, Matplotlib, SciPy
* *   **Platform**: GitHub 

## 6. Hypothesis Testing Summary

### Test 1: Sleep Duration vs Stress Level 
- **Test Type:** One-Way ANOVA
- **Result:**  
  F-statistic = 0.153, p-value = 0.859
- **Conclusion:**  
  No significant difference in stress levels across sleep duration categories.

---

### Test 2: Caffeine Intake vs Sleep Quality
- **Test Type:** Pearson Correlation
- **Result:**  
  Correlation Coefficient = –0.006, p-value = 0.889
- **Conclusion:**  
  No significant correlation found between caffeine intake and sleep quality.

---

### Test 3: Screen Time vs Sleep Quality 
- **Test Type:** Pearson Correlation
- **Result:**  
  Correlation Coefficient = 0.009, p-value = 0.834
- **Conclusion:**  
  No significant correlation found between screen time and sleep quality.

---

### Test 4: Physical Activity vs Sleep Quality 
- **Test Type:** Pearson Correlation
- **Result:**  
  Correlation Coefficent=-0.013508830985428627,p-value=0.7631671692880456
  - **Conclusion:**  
   No significant correlation found between physical activity and sleep quality.

---
## 7. Limitations and Future Work
The survey is self-reported and may continue bias.

**Future work could involve:**
- **Nested Cross-Validation:** To guard against overfitting and obtain more reliable performance estimates across different folds and hyperparameter settings.  
- **SHAP Analysis:** To open the “black box” of tree-based models, quantify feature contributions, and explain individual predictions.  
- **Ensemble Stacking:** To combine the strengths of multiple classifiers (logistic regression, random forest, gradient boosting) for potentially higher accuracy and robustness.  
- **Including academic performance metrics** (e.g. GPA, study hours) to explore their interaction with sleep and well-being.  
- **Expanding the sample size** for more robust modeling and more generalizable results.

