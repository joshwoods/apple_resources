

- Create ML
- MLDecisionTreeClassifier
-  predictions(from:) Deprecated

Instance Method

# predictions(from:)

Classifies the provided data into the target categories.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–13.0DeprecatedvisionOS 1.0+

``` source
func predictions(from data: MLDataTable) throws -> MLUntypedColumn
```

Deprecated

Use DataFrame instead of MLDataTable.

## Parameters 

`data`  

The data you want the model to classify.

## Return Value

A column of labels predicted by the classifier.

## See Also

### Testing a decision tree classifier

func predictions(from: DataFrame) throws -> AnyColumn

Predicts a column of labels for the given testing data.

