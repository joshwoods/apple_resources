

- Create ML
- MLRandomForestClassifier
- MLRandomForestClassifier.ModelParameters
- MLRandomForestClassifier.ModelParameters.ValidationData
-  MLRandomForestClassifier.ModelParameters.ValidationData.none 

Case

# MLRandomForestClassifier.ModelParameters.ValidationData.none

Do not set validation data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 16.0+visionOS 1.0+

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

Validation data provided in a DataFrame.

