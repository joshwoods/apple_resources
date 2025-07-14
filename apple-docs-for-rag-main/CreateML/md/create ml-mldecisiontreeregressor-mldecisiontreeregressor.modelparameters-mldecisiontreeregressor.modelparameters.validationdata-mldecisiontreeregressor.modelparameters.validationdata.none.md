

- Create ML
- MLDecisionTreeRegressor
- MLDecisionTreeRegressor.ModelParameters
- MLDecisionTreeRegressor.ModelParameters.ValidationData
-  MLDecisionTreeRegressor.ModelParameters.ValidationData.none 

Case

# MLDecisionTreeRegressor.ModelParameters.ValidationData.none

Do not set validation data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
case none
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generate validation data by splitting the training dataset. This is the default.

case table(MLDataTable)

Set validation data from the MLDataTable provided.

case dataFrame(DataFrame)

Set validation data from the DataFrame provided.

