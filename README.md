# Effects of Sleep Patterns on the Life Quality Of College Students

## 1. Project Overview
This project investigates the relationship between sleep patterns and the life quality of university students. It aims to assess how sleep duration, regularity, and quality correlate with well-being indicators such as caffeine intake, screen time, physical activity, stress levels and other indicators.The data will be gathered from a self-reported survey and enriched using public datasets, then the data will be analyzed using exploratory and statistical methods.

I will test the validity of the following hypothesis:

Null Hypothesis (H₀): There is no significant relationship between sleep patterns and well-being indicators among university students.

Alternative Hypothesis (H₁): There is a significant relationship between sleep patterns and well-being indicators among university students.

| Well-being Variables     | Sleep Variables               |
|--------------------------|------------------------------------|
| Stress Level             | Sleep Quality                      |
| Sleep Difficulty         | Sleep Quality                      |
| Screen Time              | Sleep Quality                      |
| Caffeine Intake          | Sleep Quality                      |
| Physical Activity Level  | Sleep Quality                      |


## 2. Motivation
I noticed that university students often suffer from irregular sleep schedules and high stress, especially during midterm weeks and finals. Understanding how sleep affects mental well-being can help students adopt healthier habits and improve academic performance and quality of life. Furthermore, I plan to better understand the data science concepts that we have learned during lectures by applying these concepts into daily life situations that concern many students such as myself.

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

## 4. Data Analysis Plan
* *   **Exploratory Analysis**: Analyze sleep duration, consistency, bedtime vs wake-up patterns.
* *   **Hypothesis Testing**: Use hypothesis testing to assess links between sleep and mental well-being scores.
* *   **Visualization**: Use bar plots, heatmaps, and scatter plots to illustrate findings.
* *   **Modeling**: Apply logistic regression to predict stress/anxiety levels from sleep features.

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
The survey data is self-reported and may contain bias  due to subjective perception.
* *   Future work could involve:
  * *  Including academic performance metrics (GPA, study hours)
  * *  Expanding sample size for more robust modeling.
  
