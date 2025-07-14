

- Create ML
- MLBoostedTreeClassifier
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Evaluates the classifier on the provided labeled data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func evaluation(on labeledData: DataFrame) -> MLClassifierMetrics
```

## Parameters 

`labeledData`  

A `DataFrame` to evaluate the trained model on.

## Return Value

Metrics that describe the classification errors (classificationError), the precision and recall percentages (precisionRecall), and a table that describes how labels were misapplied (confusion) on the provided data.

## Discussion

Evaluation should be done on a testing data set that the model has not seen as part of the training or validation data sets. The data should have feature columns with identical name and type to the training data, as well as a labels column with the same name.

## See Also

### Evaluating the boosted tree classifier

func evaluation(on: MLDataTable) -> MLClassifierMetrics

Evaluates the classifier on the provided labeled data.

Deprecated

