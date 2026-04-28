# Diabetes-Risk-Prediction

## Background Info on Diabetes

Diabetes is one of the most prevalent chronic diseases in the United States and affects millions of individuals. This disease is characterized by the body's inability to properly regulate blood glucose levels, which is either because of insufficient insulin production or reduced insulin sensitivity. Over time, unmanaged diabetes can lead to very serious complications like cardiovascular disease, kidney failure, vision loss, and reduced life expectancy. Early identification of diabetes risk factors is important for implementing preventative strategies like lifestyle changes and medical intervention.

The dataset used in this project is derived from the Behavioral Risk Factor Surveillance System (BRFSS), a large scale health survey conducted anually by the CDC. It includes self-reported information on health behaviors, chronic conditions, and demographic factors. The version used in this analysis contains over 70,000 observations and includes key indicators like body mass index (BMI), physical activity, smoking status, and history of conditions like high blood pressure and heart diseases. These variables paint a picture of individual health profiles and are perfect for predictive modeling.

For this analysis, we use a cleaned and preprocessed subset of the data that includes 21 relevant health indicators.
Specifically, we use the balanced binary version of the dataset, which has the target variable indicating whether an individual has diabetes or is at risk (including pre-diabetes). This version was selected over the original multiclass dataset because it provides a balanced class distribution, which improves the performance and interpretability of our classification models. Using a binary outcome also simplifies evaluation metrics and allows for clearer interpretation of results.

## Research Question
The goal of this project is to investigate whether patterns in health-related behaviors and conditions can be used to accurately predict diabetes risk.

Question: **Can clustering individuals into health-risk profiles using k-Means improve the performance and interpretability of a kNN model in predicting diabetes?**


To answer this question, we first build a baseline kNN model using the original health indicators. We then optimize the model through hyperparameter tuning. Next, we apply k-Means clustering to identify groups of individuals with similar health characteristics. Finally, we evaluate whether adding cluster membership as an additional feature improves diabetes prediction performance.
