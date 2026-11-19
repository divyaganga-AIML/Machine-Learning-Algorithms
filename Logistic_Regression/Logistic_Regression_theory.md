## Logistic Regression
**What is Logistic Regression?**

Logistic regression is a supervised machine learning method used to model the probability of a categorical outcome.
Most commonly binary outcomes such as ***yes/no*** or ***0/1*** by applying the sigmoid function to a linear combination of input features.


## How It Works

• **Linear Combination:** It first computes a standard linear combination of the input features 
    <img width="285" height="58" alt="image" src="https://github.com/user-attachments/assets/ad5f3dfa-8594-45f1-8671-d29451898bbb" />

• **Sigmoid Function:** It passes that linear output through the sigmoid function (or logistic function), which squashes any real number into an S-shaped curve between 0 and 1.

<img width="300" height="128" alt="image" src="https://github.com/user-attachments/assets/e60251a6-1639-4af0-890f-a120fce7379e" />

<img width="400" height="200" alt="image" src="https://github.com/user-attachments/assets/22789a52-483f-4e5d-a223-c2062943ec22" />

• **Probability & Decision Boundary:** The resulting number represents a probability. A threshold (typically 0.5) is applied to assign the input to a specific class (e.g., values ≥ 0.5 become Class 1, and < 0.5 become Class 0).

The decision boundary is the set of points where the model switches its predicted class.

Logistic regression predicts:

Class 1 when p≥0.5

Class 0 when p<0.5

<img width="300" height="150" alt="image" src="https://github.com/user-attachments/assets/8871f68b-0bba-4aca-828c-ea4ad5acc2ad" />

• **Maximum Likelihood Estimation (MLE):** logistic regression estimates its parameters using MLE (or gradient descent) to maximize the likelihood of observing the given data.

## Types of Logistic Regression

• ***Binary Logistic Regression:*** Two possible discrete outcomes (e.g., pass/fail, win/lose).

• ***Multinomial Logistic Regression:*** Three or more unordered outcomes (e.g., predicting whether an image is a cat, dog, or rabbit).

• ***Ordinal Logistic Regression:*** Three or more ordered outcomes (e.g., customer satisfaction rating from 1 to 5)

## Use cases of logistic regression
• ***Fraud detection:*** Flags data anomalies to catch financial fraud and remove fake SaaS accounts.

• ***Disease prediction:*** Predicts illness likelihood to help healthcare providers set up preventive care.

• ***Churn prediction:*** Identifies employees or clients likely to leave, prompting retention strategies.

## Core Evaluation Metrics

***Confusion Matrix:***
A confusion matrix summarizes correct and incorrect predictions:

True Negative (TN) — correctly predicted negative

False Positive (FP) — predicted positive but actually negative

False Negative (FN) — predicted negative but actually positive

True Positive (TP) — correctly predicted positive

<img width="400" height="200" alt="image" src="https://github.com/user-attachments/assets/bc6621aa-c3df-4d8c-a642-406c91968860" />

This matrix is the foundation for most other metrics. 

***Accuracy:***
Measures overall correctness

Accuracy = (TP + TN) / Total predictions

Best when classes are balanced. 

***Precision:***
Precision = TP / (TP + FP)

High precision means fewer false alarms—important in spam detection or fraud detection. 

***Recall:*** Recall = TP / (TP + FN)

High recall means fewer missed positives—critical in medical diagnosis. 

***F1‑Score:*** Harmonic mean of precision and recall.

Useful when you need balance between avoiding false positives and false negatives. 

F1=2× (precision+recall)/(precision×recall)

​
 ***ROC Curve & AUC:***

ROC curve plots True Positive Rate vs. False Positive Rate across thresholds.

AUC measures how well the model separates classes; higher is better.

Ideal for comparing models or evaluating performance across thresholds.

<img width="286" height="200" alt="image" src="https://github.com/user-attachments/assets/2a23c5f0-b8ab-4b3a-a7ed-6a3d800e5b22" />
<img width="280" height="200" alt="image" src="https://github.com/user-attachments/assets/f520d5bc-3984-4614-a1c2-60548bbae484" />




**Practical Implementation of Logistic Regression using Bank data:**
Logistic_regression_example.ipynb


