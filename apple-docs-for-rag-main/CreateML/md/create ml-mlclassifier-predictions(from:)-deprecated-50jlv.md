

- Create ML
- MLClassifier
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

## Discussion

If the supplied data doesn’t match the expected columns (noted by the featureColumns property), this method throws an MLCreateError.type(reason:).

## See Also

### Testing a classifier

func predictions(from: DataFrame) throws -> AnyColumn

