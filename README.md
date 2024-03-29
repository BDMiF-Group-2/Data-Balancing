# Data-Balancing

Used under sampling and over sampling methods to handle with data imbalance.
Over sampling is significantly recommended.
ADASYN is more recommended since it reduces bias from synthetic data, comparing to SMOTE.

1.0 update:
  In order to find out an optimal K value for ADASYN (KNN based), an iteration from k = 1 to 80 was conducted with python.
  R has spent an hour to run an iteration of 10 and is yet finished.
  Notion: to find the minimum error rate (defined by the proportion of wrong predictions to test values)
  Model: KNN
  Training and testing data: original dataset, with train test ratio = 0.8 : 0.2
  No data preprocessing was conducted
  Result: k = [1, 2, 3, 5, 7] have higher error rate, comparing to the rest. Minimun error rate = 0.030058651026392963

  It is recommended to choose k = 9 as a minimum odd k value, or k = 79 as the closest typical value sqrt(6599 - 220)
