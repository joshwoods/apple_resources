

- Create ML
- MLRegressor
-  evaluation(on:) Deprecated

Instance Method

# evaluation(on:)

Evaluates the classifier on the provided labeled data.

macOS 10.14–13.0Deprecated

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

### Evaluating a regressor

func evaluation(on: DataFrame) -> MLRegressorMetrics

Evaluates the classifier on the provided labeled data.

