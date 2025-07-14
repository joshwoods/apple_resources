

- Create ML
- MLRegressor
-  predictions(from:) Deprecated

Instance Method

# predictions(from:)

Predicts the target value from the provided data.

macOS 10.14–13.0Deprecated

``` source
func predictions(from data: MLDataTable) throws -> MLUntypedColumn
```

Deprecated

Use DataFrame instead of MLDataTable.

## Parameters 

`data`  

The data you want the model to make predictions from.

## Return Value

A column of values predicted by the regressor.

## Discussion

If the supplied data doesn’t match the expected columns (noted by the featureColumns property), this method throws an MLCreateError.type(reason:).

## See Also

### Testing a regressor

func predictions(from: DataFrame) throws -> AnyColumn

