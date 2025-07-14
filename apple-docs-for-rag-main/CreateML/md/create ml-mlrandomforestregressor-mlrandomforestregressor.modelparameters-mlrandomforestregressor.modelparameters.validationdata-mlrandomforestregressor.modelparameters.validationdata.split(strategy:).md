

- Create ML
- MLRandomForestRegressor
- MLRandomForestRegressor.ModelParameters
- MLRandomForestRegressor.ModelParameters.ValidationData
-  MLRandomForestRegressor.ModelParameters.ValidationData.split(strategy:) 

Case

# MLRandomForestRegressor.ModelParameters.ValidationData.split(strategy:)

Generate validation data by splitting the training dataset. This is the default.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
case split(strategy: MLSplitStrategy)
```

## See Also

### Specifying validation data

case table(MLDataTable)

Set validation data from the MLDataTable provided.

case dataFrame(DataFrame)

Set validation data from the DataFrame provided.

case none

Do not set validation data.

