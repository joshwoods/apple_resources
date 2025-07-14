

- Create ML
- MLLinearRegressor
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Evaluates the classifier on the provided labeled data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func evaluation(on labeledData: DataFrame) -> MLRegressorMetrics
```

## Parameters 

`labeledData`  

A `DataFrame` to evaluate the trained model on.

## Return Value

Metrics that describe the maximum error (maximumError) or the average error (rootMeanSquaredError).

## Discussion

Evaluation should be done on a testing data set that the model has not seen as part of the training or validation data sets. The data should have feature columns with identical name and type to the training data, as well as a labels column with the same name.

## See Also

### Evaluating a Linear Regressor

func evaluation(on: MLDataTable) -> MLRegressorMetrics

Evaluates the classifier on the provided labeled data.

Deprecated

