# Issue: Error When Fitting Training Dataset into a Decision Tree Classifier

## Problem Description

I am working on the machine learning assignment and attempting to fit my training dataset (`X_train`) into a Decision Tree Classifier using scikit-learn. However, when I execute the `fit` method, I encounter an error.

## Code

```python
# Import necessary modules
from sklearn.tree import DecisionTreeClassifier
import numpy as np

# Create a training dataset with mismatched shapes
X_train = np.array([[1, 2], [3, 4], [5, 6]])
y_train = np.array([0, 1])

# Initialize the Decision Tree Classifier
clf = DecisionTreeClassifier()

# Try to fit the model
try:
    clf.fit(X_train, y_train)
except Exception as e:
    print(f"An error occurred: {e}")
```

## Error
```
An error occurred: Number of labels=2 does not match number of samples=3
```
