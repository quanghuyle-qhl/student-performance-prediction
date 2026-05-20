# Predictive Analytics for Early Identification of Academic Risk in Primary Education
## Executive Summary
The number of Year 3 students identified as at risk in writing increased significantly from 25.7% in 2016 to 36.3% in 2021, highlighting a growing concern for both student achievement and school performance. This project focuses on identifying key factors that contribute to writing difficulties and developing early intervention strategies to better support students.
#### Key Findings
Cognitive disabilities, literacy, and numeracy skills were identified as major predictors of writing risk.
Early intervention can help improve student outcomes and reduce long-term academic challenges.
Recommended strategies are expected to reduce at-risk students by 20–30% within 3 years.
#### Future Improvements
Collaborate with schools to continuously collect updated student data.
Refine predictive models to improve accuracy and reliability.
Explore additional variables and intervention approaches to strengthen decision-making and student support.
## Business Problem
The percentage of Year 3 students at risk in writing increased from 25.7% in 2016 to 36.3% in 2021, creating concerns for student academic success and the school’s overall performance and reputation. The school requires a predictive solution to identify at-risk students early and allocate educational support effectively. The project addresses this challenge by leveraging machine learning to improve intervention strategies and reduce the number of at-risk students.
## Methodology
The project applied both supervised and unsupervised machine learning approaches:
- Logistic Regression for interpretable binary classification.
- k-Nearest Neighbors (k-NN) for similarity-based classification.
- k-Means Clustering for grouping students with similar learning characteristics.

The dataset contained 2,000 students and 34 attributes related to demographics, literacy, numeracy, disability conditions, and school background. Data preprocessing included:
- Handling anomalies and missing values.
- Encoding categorical variables.
- Feature selection based on correlation analysis.
- Scaling numerical variables.
- Splitting data into 80% training and 20% testing sets.

Model performance was evaluated using Accuracy, Precision, Recall, F1-score, ROC-AUC, and 10-fold cross-validation.
## Demonstration of Skills and Capabilities
**Data-Driven Feature Selection:** Identified that literacy and numeracy assessments, particularly TextLevel, Clay, Counting, and Writing Vocabulary scores, have strong relationships with Year 3 writing risk, while school background and SES factors showed weaker predictive influence.

**Statistical & Machine Learning Analysis:** Applied Logistic Regression, k-NN, and k-Means Clustering to predict and segment at-risk students. Logistic Regression coefficients were analysed to demonstrate how factors such as cognitive disabilities, literacy performance, and numeracy skills influence writing risk.

**Model Optimisation & Evaluation:** Compared models using Accuracy, Precision, Recall, F1-score, ROC-AUC, and 10-fold cross-validation to determine the most suitable solution for identifying at-risk students while balancing false positives and missed cases.

**Exploratory Data Analysis & Visualisation:** Conducted univariate, bivariate, and multivariate analysis using heatmaps, boxplots, histograms, ROC curves, and clustering visualisations to uncover patterns and relationships within student performance data.

**Technical Literacy & Data Processing:** Managed complex educational variables including disability conditions, literacy assessments, numeracy assessments, and demographic information to build a multidimensional predictive model.

**Business Translation & Educational Insight:** Converted machine learning findings into practical educational recommendations, including early intervention strategies, literacy and numeracy support programs, and targeted assistance for cognitively disadvantaged students.
## Results and Business Recommendations
Logistic Regression outperformed k-NN with:
- Accuracy: 74.75%
- Precision: 65.68%
- AUC: 0.79

Key findings showed that:
- Cognitive disabilities strongly increase writing risk.
- Higher literacy and numeracy performance reduce writing risk.
- Students with low Clay and Counting scores are more likely to underperform in writing.

Business recommendations include:
- Early intervention programs for students with cognitive disabilities.
- Strengthening literacy and numeracy support programs.
- Providing targeted support for students with weak reading comprehension and foundational math skills.
- Using the predictive model to assist educators in identifying at-risk students earlier.
## Model Integrity & Risk Assessment
The models were validated using 10-fold cross-validation to ensure reliability and consistency. Logistic Regression showed stable performance across validation folds. However, the model’s recall score (~50%) indicates that some at-risk students may still not be identified, creating a risk of missed interventions.

Additional risks and limitations include:
- Small dataset size (2,000 records).
- Limited ability to capture complex feature interactions.
- Moderate cluster separation in k-Means clustering.
- Potential performance decline if the model is not regularly retrained with updated data.

To reduce these risks, teacher reviews and ongoing model monitoring were recommended alongside automated predictions.
## Context and Credit
Client: Data2Intel (Simulated)

Tools used: Python, Google Colab

Analyst: Quang Huy Le
