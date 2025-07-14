

- Create ML
- MLLogisticRegressionClassifier
- MLLogisticRegressionClassifier.ModelParameters
- MLLogisticRegressionClassifier.ModelParameters.ValidationData
-  MLLogisticRegressionClassifier.ModelParameters.ValidationData.table(\_:) 

Case

# MLLogisticRegressionClassifier.ModelParameters.ValidationData.table(\_:)

Set validation data from the MLDataTable provided.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 10.15–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0+

``` source
case table(MLDataTable)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generate validation data by splitting the training dataset. This is the default.

case dataFrame(DataFrame)

Validation data provided in a DataFrame.

case none

Do not set validation data.

