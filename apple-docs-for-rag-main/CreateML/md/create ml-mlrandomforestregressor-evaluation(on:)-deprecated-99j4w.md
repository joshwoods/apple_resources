

- Create ML
- MLRandomForestRegressor
-  evaluation(on:) Deprecated

Instance Method

# evaluation(on:)

Evaluates the classifier on the provided labeled data.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–13.0DeprecatedvisionOS 1.0+

``` source
func evaluation(on labeledData: MLDataTable) -> MLRegressorMetrics
```

Deprecated

Use DataFrame instead of MLDataTable.

## Parameters 

`labeledData`  

An `MLDataTable` to evaluate the trained model on.

## Return Value

Metrics that describe the maximum error (maximumError) or the average error (rootMeanSquaredError).

## Discussion

Evaluation should be done on a testing data set that the model has not seen as part of the training or validation data sets. The data should have feature columns with identical name and type to the training data, as well as a labels column with the same name.

## See Also

### Evaluating a Random Forest Regressor

func evaluation(on: DataFrame) -> MLRegressorMetrics

Evaluates the classifier on the provided labeled data.

