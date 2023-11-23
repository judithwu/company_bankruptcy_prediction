# Predicting company bankruptcy
Predicted company bankrupty with Random Forest Classifier.   
Started with a model of 100 estimators and a max depth of 5, achieved 92% accuracy.   
Then used RandomizedSearchCV to find better hyperparameters, achieving 96% accuracy with 100 estimators and a max depth of 20.  
With the tuned model, the false negative rate (predicted not bankrupt when, in fact, you are bankrupt) decreased; however, the amount of true positives decreased, and false positive rate increased (predicted bankrupt when, in fact, you are not bankrupt). But in the context of this problem, it seems worse to predict you are not bankrupt when in reality you are, than predicting you are bankrupt when you are actually not, so this trade off seemed reasonable.   
The 5 most important features in predicting company bankruptcy was concluded to be total debt/total net worth, borrowing dependency, net income to total assets, total income/total expense, and persistent earnings per share (EPS) in the last four seasons.
