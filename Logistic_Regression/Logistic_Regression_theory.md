## Logistic Regression
**What is Logistic Regression?**

Logistic regression is a supervised machine learning method used to model the probability of a categorical outcome.
Most commonly binary outcomes such as ***yes/no*** or ***0/1*** by applying the sigmoid function to a linear combination of input features.


## How It Works

• **Linear Combination:** It first computes a standard linear combination of the input features 
    <img width="285" height="58" alt="image" src="https://github.com/user-attachments/assets/ad5f3dfa-8594-45f1-8671-d29451898bbb" />

• **Sigmoid Function:** It passes that linear output through the sigmoid function (or logistic function), which squashes any real number into an S-shaped curve between 0 and 1.

<img width="400" height="200" alt="image" src="https://github.com/user-attachments/assets/22789a52-483f-4e5d-a223-c2062943ec22" />

• **Probability & Decision Boundary:** The resulting number represents a probability. A threshold (typically 0.5) is applied to assign the input to a specific class (e.g., values ≥ 0.5 become Class 1, and < 0.5 become Class 0).

• **Maximum Likelihood Estimation (MLE):** logistic regression estimates its parameters using MLE (or gradient descent) to maximize the likelihood of observing the given data.

## Types of Logistic Regression

• ***Binary Logistic Regression:*** Two possible discrete outcomes (e.g., pass/fail, win/lose).

• ***Multinomial Logistic Regression:*** Three or more unordered outcomes (e.g., predicting whether an image is a cat, dog, or rabbit).

• ***Ordinal Logistic Regression:*** Three or more ordered outcomes (e.g., customer satisfaction rating from 1 to 5)

## Use cases of logistic regression
• ***Fraud detection:*** Flags data anomalies to catch financial fraud and remove fake SaaS accounts.

• ***Disease prediction:*** Predicts illness likelihood to help healthcare providers set up preventive care.

• ***Churn prediction:*** Identifies employees or clients likely to leave, prompting retention strategies.
