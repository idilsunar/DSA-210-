# DSA-210-
**The Impact of Screen Time on Children\'s Brain Development**

### **1. Project Overview**

I am a student from Sabancı University, and this is the proposal for my
term project for DSA210. The aim of this project is to gain a better
understanding of how screen time affects the development of children. I
will be analyzing data from datasets such as ABCD and NHANES.
Furthermore, I will be enriching the data obtained by incorporating
additional data sources related to child healthcare, educational
performance, and behavioral assessments to enhance the analysis and
provide deeper insights.

My main goal is to shed light on how screen time influences children\'s
development, with a particular focus on brain development. I will be
talking about brain development in terms of cognitive processes and
educational performance. Additionally, I will develop a Screen Time
Impact Score (STIS) by integrating various cognitive, academic, and
social development metrics to provide a more comprehensive research on
how screen time affects children.

### **2. Motivation**

My motivation for conducting this research is to provide 
a better understanding of how screen time affects children\'s brain development. 
Lately digital devices have become an integral part of children's daily lives, 
therefore I believe that it is very important to research their impact on their health 
and establish guidelines for healthy usage. The development of Screen Time Impact Score
(STIS) is aimed to make the understanding of screen time's effects on children for 
policymakers and parents easier. This way, they can set more appropriate screen time 
limits while ensuring a balance with other activities that help children develop. 
This research can also provide insight to many people such as myself who want to learn
more about digital exposure's effects on cognitive processes and educational performance
in children. By doing this project, I aim to better understand the concepts of data 
science that we have learned in class by applying them to real life scenarios as well 
as gain more knowledge on the correlation between screen time and children's brain 
development.

### 

### **3. Data Sources**

For this project, I will use publicly available datasets and enrich them
with supplementary data sources. My primary datasets are as listed
below:

**The Adolescent Brain Cognitive Development (ABCD) Study** -- A
large-scale longitudinal dataset providing information on brain imaging,
cognitive functions, and lifestyle habits of children.

**National Health and Nutrition Examination Survey (NHANES)** --
Includes self-reported screen time usage and cognitive assessments.

### **4. Data Enrichment** 

To enhance the datasets that I will be using, I will integrate data from
healthcare, academic, and behavioral studies. The enriched dataset will
allow for a more comprehensive analysis of how screen time influences
different aspects of child brain development.

#### **Cognitive Processes Metrics**

1.  **Memory (Short-term & Working Memory):** Measured using ABCD
    cognitive tasks.

2.  **Attention Span:** Behavioral tests and survey data from
    ABCD/NHANES.

3.  **Executive Function (Decision-making, Self-control):** Brain
    imaging and response inhibition tasks.

4.  **Processing Speed:** Tasks requiring rapid decision-making.

#### **Academic Performance Metrics**

1.  **Standardized Test Scores:** Math, Reading Comprehension, and
    Critical Thinking scores.

2.  **Homework Completion & Study Habits:** Self-reported data from
    educational datasets.

3.  **Classroom Engagement:** Behavioral assessment surveys and
    teacher-reported engagement levels.

### **5. Development of the Screen Time Impact Score (STIS)**

To quantify the impact of screen time on children, I will develop the
Screen Time Impact Score (STIS), which will combine multiple cognitive
and academic factors.

I plan to conduct my calculations using python, exporting numpy and
pandas libraries.

#### **Formula:**

STIS=α(−screen time)+β(cognitive test score)+γ(academic performance)

STIS can be interpreted using a scale from 0-100.The scores from 0-30
pose a low risk while 31-50 pose a moderate risk with some negative
effects observed, 51-70 present a high risk with significant negative
impacts, and scores between 71-100 have a severe risk.

### **6. Project Plan**

1.  **Data Collection:** Retrieve data from ABCD, NHANES, and
    supplementary sources and supplementary sources such as NIH
    repositories, Kaggle datasets, and Google Dataset Search. Identify
    relevant features including screen time duration, cognitive test
    scores, academic performance, and social responsiveness from
    collected datasets.

2.  **Data Cleaning:** Identify and remove outliers using z-score
    analysis. Normalize and standardize numerical features to ensure
    uniformity across different datasets.

3.  **Exploratory Data Analysis:** Identify patterns and correlations
    using statistical visualization tools such as Matplotlib and
    Seaborn. Use heatmaps to explore correlations between variables.

4.  **Hypothesis Testing:** Test relationships between screen time and
    cognitive measures such as attention span, memory retention, and
    emotional regulation.

5.  **Machine Learning Models:** Build predictive models to analyze the
    impact of screen exposure on brain development.

6.  **STIS:** To create STIS, first I will select the most relevant
    variables contributing to screen time's impact, including screen
    time per day, cognitive test scores, academic performance metrics.
    Next,the weight assignment will be conducted using Principal
    Component Analysis (PCA) to determine the most influential factors
    (α, β, γ). For the score calculation, all values will be normalized
    on a 0-100 scale to ensure comparability, and the weighted formula
    will be applied.

7.  **Visualization:** Create charts and heatmaps to illustrate trends
    and findings by using Matplotlib and Seaborn.

**7. Tools and Technologies**

> 1.**Programming Language:** Python.
>
> 2.**Libraries:** Pandas, NumPy, Matplotlib, Seaborn.
>
> 3.**Data Sources:** NIH data repositories, Kaggle, government health
> databases, Google Dataset Search.
>
> 4.**Platform for Documentation & Version Control:** GitHub.
