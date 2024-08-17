# Home Credit Default Risk - Kaggle Competition 

## Group members
Varsha Ravi Varma - varavi@iu.edu

Athulya Anand - athanand@iu.edu

Shubham Patil - shupatil@iu.edu

Sricharraan Ramaswamy - sriramas@iu.edu

## Abstract
Based in 1997, Home Credit International is a global consumer finance company with operations in ten countries. Due to poor or no credit histories, it is difficult for many people to get loans, and unfortunately, these individuals are often exploited by unreliable lenders. Financial inclusion is at the core of the mission of companies such as Home Credit, which provides borrowers with a positive and secure borrowing experience. Although Home Credit currently uses various statistical and machine learning methods to predict their clients' repayment abilities, they are hoping a new model can be developed that will ensure borrowers who can repay are not rejected, allowing them to succeed. The challenge is to construct a model that can predict the level of risk associated with an individual loan. With this project, we intend to use historical loan application data to predict whether or not a borrower will be able to repay a loan.

## Data
● Application_train / Application_test: is the main training and testing database of Home Credit loan applications. Loans are identified by the feature SK_ID_CURR, which is a row identifier. Data from the training application contains TARGET information indicating 0: the loan was repaid or 1: the loan was not repaid.

● Bureau: information pertaining to previous credit from other financial institutions. Every previous credit has its own row in the bureau, but one loan can have multiple credit histories.

● Bureau_balance: monthly data regarding previous credits in the bureau. Each row represents one month of a previous credit, and a previous credit can have multiple rows, one for each month of the credit duration.

 ● previous_application: previous applications for loans at Home Credit of clients who have loans in the application data. A loan may have more than one previous application. Previous applications are identified by the feature SK_ID_PREV and contain a row.
 
● POS_CASH_BALANCE: data regarding previous point-of-sale or cash loans that clients have requested from Home Credit. A row represents one month of a previous point of sale or cash loan. A loan can have many rows.

● credit_card_balance: monthly data about previous credit cards clients have had with Home Credit. Each row represents a credit card balance for one month, and a single credit card may have several rows.

● Installments_payments: payment history for previous loans with Home Credit. There is one row for each payment made and one row for each missed payment.

## Modeling
Machine learning algorithms play an important role in achieving the desired results. To achieve the best accuracy, we have selected three algorithms from which to derive results.

● Naive Bayes: Naive Bayes is based on Bayes's Theorem and the assumption of independence between predictors. This algorithm is particularly useful with such a large dataset because the model is easy to build, with no complicated iterative parameter estimation.

● Logistic Regression: Logistic regression predicts the likelihood of a dichotomous outcome. It is based on using one or more predictors. This method produces a logistic curve whose range is limited to values between 0 and 1.

● Random Forest: This model can be used for both classification and regression. Put the input vector down each tree in the forest in order to classify a new object from the input vector. Ultimately, it is the classification with the greatest number of votes that is selected. The accuracy of the method will be compared with that of logistic regression in the test case

## Metrics
For this classification problem, we are planning to use the following performance metrics depending on the training model:

● Accuracy: Accuracy is defined as the ratio of correctly classified points to the total number of points.

● Confusion Matrix: A confusion matrix is a summary of predicted results in a specific table layout that provides a visual representation of the machine learning model's performance.

● F-1 Score: The F1 score is the arithmetic mean of precision and recall.

● Log Loss: A logarithmic loss (or log loss) is a way to measure the performance of a classification
model, where the prediction is a probability value between 0 and 1.

● ROC AUC: The Receiver Operating Characteristic curve, or ROC curve, is derived by plotting the
True Positive (TP) against the False Positive (FP) at various threshold settings.
