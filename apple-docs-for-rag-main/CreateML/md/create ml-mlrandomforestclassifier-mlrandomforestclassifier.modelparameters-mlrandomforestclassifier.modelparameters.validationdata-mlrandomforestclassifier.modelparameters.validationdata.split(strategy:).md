

- Create ML
- MLRandomForestClassifier
- MLRandomForestClassifier.ModelParameters
- MLRandomForestClassifier.ModelParameters.ValidationData
-  MLRandomForestClassifier.ModelParameters.ValidationData.split(strategy:) 

Case

# MLRandomForestClassifier.ModelParameters.ValidationData.split(strategy:)

Generate validation data by splitting the training dataset. This is the default.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 16.0+visionOS 1.0+

``` source
case split(strategy: MLSplitStrategy)
```

## See Also

### Specifying validation data

case table(MLDataTable)

Set validation data from the MLDataTable provided.

case dataFrame(DataFrame)

Validation data provided in a DataFrame.

case none

Do not set validation data.

