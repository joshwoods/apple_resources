

- Create ML
- MLSupportVectorClassifier
-  predictions(from:) Deprecated

Instance Method

# predictions(from:)

Classifies the provided data into the target categories.

macOS 10.14–13.0Deprecated

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

### Testing a support vector classifier

func predictions(from: DataFrame) throws -> AnyColumn

Predicts a column of labels for the given testing data.

Deprecated

