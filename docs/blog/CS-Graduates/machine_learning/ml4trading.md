---
title: ML4T
title_full: Machine Learning for Trading
description: Machine Learning algorithms and its application
tags:
  - Algorithms
  - Machine-Learning
  - Trading
  - OMSCS
---

## Machine Learning for Trading

[7646 ML4T](http://lucylabs.gatech.edu/ml4t/)

### Book References

[machine-learning-for-trading](https://github.com/stefan-jansen/machine-learning-for-trading)

[What Hedge Funds Really Do by Romero and Balch](https://learning.oreilly.com/library/view/what-hedge-funds/9781631570896/)

[Machine Learning, Tom Mitchell](https://www.amazon.com/gp/product/0070428077/ref=as_li_tlie=UTF8&camp=1789&creative=9325&creativeASIN=0070428077&linkCode=as2&tag=teambotsorg&linkId=TMHMI7I43WHC4O3X)


## Random Forest & Q-Learner Strategy Learner

Final project for 3 different types of ML: Decision Trees, reinforcement learning, optimization.

Quantative factors X, dependant variable Y.

### Regression Trees

X1, X2, X3 -> Regression model -> Y

1. Roll back to the beginning of data to get training data.
2. Measure X1, X2, X3 data, not peek forward, only use data until the date.
3. Build the model: Decision Trees, reinforcement learning, optimization.

Drawbacks:

Cannot distinguish between

* Uncertain large return
* Certain small return
* When doing nothing is smart

Don't know when to exit.

### Reinforcement learning.

## Q&A

### What should we consider in manual strategy?

Align the API.

### Is it useful normalizing the indicators?

Decision Tree could have not standardized indicators.

KNN needs to have standardized indicators.

### How to make Dyna run faster?

Use vectorizing code.

### How do we combine indicators, sequentially? Or how do we assign weight or priority in developing a strategy?

* Find threshold for each indicators. Just use the threshold, then voting
* Sequentially one by one (All should be true)
* Assign weight to each one.

Start with 1 indicator first, see if it's better to add more indicators.

