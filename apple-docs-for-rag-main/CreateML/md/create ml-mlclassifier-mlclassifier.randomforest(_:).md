

- Create ML
- MLClassifier
-  MLClassifier.randomForest(\_:) 

Case

# MLClassifier.randomForest(\_:)

A classifier based on a collection of decision trees trained on subsets of the data.

macOS 10.14+

``` source
case randomForest(MLRandomForestClassifier)
```

## Discussion

Don’t create an MLClassifier using one of its enumeration cases. Use the classifier’s initializer instead.

## See Also

### Classifier cases

case decisionTree(MLDecisionTreeClassifier)

A classifier that predicts the target by creating rules to split the data.

case boostedTree(MLBoostedTreeClassifier)

A classifier based on a collection of decision trees combined with gradient boosting.

case logisticRegression(MLLogisticRegressionClassifier)

A classifier that predicts a discrete target value as a function of data features.

case supportVector(MLSupportVectorClassifier)

A classifier that predicts a binary target value by maximizing the separation between categories.

Deprecated

