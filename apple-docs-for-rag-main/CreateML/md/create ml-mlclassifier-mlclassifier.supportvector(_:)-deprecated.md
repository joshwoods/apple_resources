

- Create ML
- MLClassifier
-  MLClassifier.supportVector(\_:) Deprecated

Case

# MLClassifier.supportVector(\_:)

A classifier that predicts a binary target value by maximizing the separation between categories.

macOS 10.14–14.0Deprecated

``` source
case supportVector(MLSupportVectorClassifier)
```

## Discussion

Don’t create an MLClassifier using one of its enumeration cases. Use the classifier’s initializer instead.

## See Also

### Classifier cases

case decisionTree(MLDecisionTreeClassifier)

A classifier that predicts the target by creating rules to split the data.

case randomForest(MLRandomForestClassifier)

A classifier based on a collection of decision trees trained on subsets of the data.

case boostedTree(MLBoostedTreeClassifier)

A classifier based on a collection of decision trees combined with gradient boosting.

case logisticRegression(MLLogisticRegressionClassifier)

A classifier that predicts a discrete target value as a function of data features.

