

- Create ML
- MLRegressor
-  MLRegressor.boostedTree(\_:) 

Case

# MLRegressor.boostedTree(\_:)

A regressor based on a collection of decision trees combined with gradient boosting.

macOS 10.14+

``` source
case boostedTree(MLBoostedTreeRegressor)
```

## Discussion

Don’t create an MLRegressor using one of its enumeration cases. Use the regressor’s initializer instead.

## See Also

### Regressor cases

case linear(MLLinearRegressor)

A regressor that estimates the target as a linear function of the features.

case decisionTree(MLDecisionTreeRegressor)

A regressor that estimates the target by learning rules to split the data.

case randomForest(MLRandomForestRegressor)

A regressor based on a collection of decision trees trained on subsets of the data.

