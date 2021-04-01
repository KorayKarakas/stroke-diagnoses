# stroke-diagnoses

## Source of data
* https://www.kaggle.com/fedesoriano/stroke-prediction-dataset

## EDA
As expected, one of the strongest correlations between the diagnosis of stroke was age however there were some other underlying health conditions that indicated a heightened probability of suffering from a stroke. The correlations aren't strong enough to suggest a direct relationship however features such as BMI and Average Glucose Level display relatively strong correlations.

The dataset has an imbalance of Female to Male patients so it's difficult to determine whether gender correlates with a diagnosis however the proportions of stroke diagnoses in this particular dataset lean towards a Female bias. 

There doesn't seem to be a direct correlation between smoking status and diagnoses. The dominating category in this feature are patients who have never smoked and the concurrent smokers have the least number of cases. However, there are underlying reasons this may be misleading such as the mean age for the dominating category being higher than the rest. Given that age demonstrates a correlation with stroke diagnoses, this is an important factor to consider.

## Classification

The dataset presents an imbalance issue with 95% of the entries belonging to the negative class and 4.8% to the minority positive class. Accuracy measures are misleading given the imbalance so other metrics have stronger consideration in this project. 

This project explores popular classification models such as: Decision Tree, Random Forest, Gaussian Naive Bayes and K-Nearest Neighbors. Files titled `SMOTE` display a method of working around the class imbalance by synthetically oversampling the training set to balance the proportions between the minority and majority class. 
