

- Create ML
- MLLinearRegressor
- MLLinearRegressor.ModelParameters
- MLLinearRegressor.ModelParameters.ValidationData
-  MLLinearRegressor.ModelParameters.ValidationData.dataFrame(\_:) 

Case

# MLLinearRegressor.ModelParameters.ValidationData.dataFrame(\_:)

Set validation data from the DataFrame provided.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
case dataFrame(DataFrame)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generate validation data by splitting the training dataset. This is the default.

case table(MLDataTable)

Set validation data from the MLDataTable provided.

case none

Do not set validation data.

