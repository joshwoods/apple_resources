

- Create ML
- MLClassifier
-  MLClassifier.decisionTree(\_:) 

Case

# MLClassifier.decisionTree(\_:)

A classifier that predicts the target by creating rules to split the data.

macOS 10.14+

``` source
case decisionTree(MLDecisionTreeClassifier)
```

## Discussion

Don’t create an MLClassifier using one of its enumeration cases. Use the classifier’s initializer instead.

## See Also

### Classifier cases

case randomForest(MLRandomForestClassifier)

A classifier based on a collection of decision trees trained on subsets of the data.

case boostedTree(MLBoostedTreeClassifier)

A classifier based on a collection of decision trees combined with gradient boosting.

case logisticRegression(MLLogisticRegressionClassifier)

A classifier that predicts a discrete target value as a function of data features.

case supportVector(MLSupportVectorClassifier)

A classifier that predicts a binary target value by maximizing the separation between categories.

Deprecated

