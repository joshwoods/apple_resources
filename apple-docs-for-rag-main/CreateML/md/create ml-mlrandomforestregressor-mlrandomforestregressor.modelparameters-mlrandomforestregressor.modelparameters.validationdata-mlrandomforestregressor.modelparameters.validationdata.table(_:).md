

- Create ML
- MLRandomForestRegressor
- MLRandomForestRegressor.ModelParameters
- MLRandomForestRegressor.ModelParameters.ValidationData
-  MLRandomForestRegressor.ModelParameters.ValidationData.table(\_:) 

Case

# MLRandomForestRegressor.ModelParameters.ValidationData.table(\_:)

Set validation data from the MLDataTable provided.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0+

``` source
case table(MLDataTable)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generate validation data by splitting the training dataset. This is the default.

case dataFrame(DataFrame)

Set validation data from the DataFrame provided.

case none

Do not set validation data.

