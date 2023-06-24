# Detecting Credit Card Fraud

## Project Objective
This project focuses on leveraging machine learning models to predict fraudulent credit card transactions. The analysis involves examining customer-level data collected and analyzed through a collaborative effort between Worldline and the Machine Learning Group. The dataset, sourced from Kaggle, comprises 284,807 transactions, with 492 identified as fraudulent. Due to the dataset's imbalanced nature, addressing this imbalance is crucial before proceeding with model development.

## Business Challenge Overview
For banks, retaining highly profitable customers stands as a top business priority. However, the persistent threat of banking fraud poses a substantial risk, leading to financial losses, erosion of trust, and credibility. The Nilson report estimated that global banking frauds would reach $30 billion by 2020. With the surge in digital payment channels, instances of fraudulent transactions are on the rise, necessitating proactive monitoring and fraud prevention mechanisms.

In the banking sector, employing machine learning for credit card fraud detection is not just a trend but a necessity. It enables institutions to implement proactive monitoring and fraud prevention mechanisms, reducing manual reviews, costly chargebacks, and denials of legitimate transactions.

## Defining Fraud in the Context of Credit Cards
Credit card fraud encompasses any dishonest act or behavior aimed at obtaining information without proper authorization from the account holder, driven by a motive for financial gain. Skimming, the duplication of information from a card's magnetic strip, is a prevalent form of fraud. Other methods include manipulation of genuine cards, creation of counterfeit cards, theft or loss of credit cards, and fraudulent telemarketing.

## Data Overview
The dataset, available for download here, includes credit card transactions made by European cardholders over two days in September 2013. Of the 284,807 transactions, 492 were identified as fraudulent. The dataset is highly unbalanced, with frauds accounting for only 0.172% of total transactions. Principal Component Analysis (PCA) has been applied to maintain data confidentiality. Features such as 'time' and 'amount' are included, along with principal components (V1 to V28) obtained through PCA. The 'time' feature represents seconds elapsed between the first transaction and subsequent ones, 'amount' denotes the transaction amount, and 'class' signifies the class label (1 for fraud, 0 for others).

## Project Workflow
The project workflow consists of the following key steps:

** Data Understanding: Load and understand the features present in the data, selecting relevant features for the final model.
** Exploratory Data Analysis (EDA): Conduct univariate and bivariate analyses, considering feature transformations if necessary. Since Gaussian variables are used, Z-scaling may not be required, but addressing skewness is recommended.
** Train/Test Split: Perform a train/test split to assess model performance with unseen data. Utilize k-fold cross-validation for validation, ensuring adequate representation of the minority class in test folds.
** Model Building/Hyperparameter Tuning: Experiment with different models and fine-tune hyperparameters to achieve the desired performance on the dataset. Explore various sampling techniques to enhance model robustness.
** Model Evaluation: Evaluate models using appropriate metrics, giving priority to accurately identifying fraudulent transactions due to the dataset's imbalanced nature. Choose evaluation metrics aligned with this business goal.