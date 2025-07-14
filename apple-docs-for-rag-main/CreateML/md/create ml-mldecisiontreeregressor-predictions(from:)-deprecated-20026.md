

- Create ML
- MLDecisionTreeRegressor
-  predictions(from:) Deprecated

Instance Method

# predictions(from:)

Predicts the target value from the provided data.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–13.0DeprecatedvisionOS 1.0+

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

## See Also

### Testing a decision tree regressor

func predictions(from: DataFrame) throws -> AnyColumn

Predicts a column of labels for the given testing data.

