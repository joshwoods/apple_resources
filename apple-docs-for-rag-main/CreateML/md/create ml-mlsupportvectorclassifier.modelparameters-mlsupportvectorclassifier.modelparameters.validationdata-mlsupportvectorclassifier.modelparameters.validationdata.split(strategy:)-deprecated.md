

- Create ML
- MLSupportVectorClassifier
- 
  - MLSupportVectorClassifier
- MLSupportVectorClassifier.ModelParameters
- MLSupportVectorClassifier.ModelParameters.ValidationData
-  MLSupportVectorClassifier.ModelParameters.ValidationData.split(strategy:) Deprecated

Case

# MLSupportVectorClassifier.ModelParameters.ValidationData.split(strategy:)

Generate validation data by splitting the training dataset. This is the default.

macOS 10.15–14.0Deprecated

``` source
case split(strategy: MLSplitStrategy)
```

## See Also

### Specifying validation data

case table(MLDataTable)

Set validation data from the MLDataTable provided.

Deprecated

case dataFrame(DataFrame)

Validation data provided in a DataFrame.

Deprecated

case none

Do not set validation data.

Deprecated

