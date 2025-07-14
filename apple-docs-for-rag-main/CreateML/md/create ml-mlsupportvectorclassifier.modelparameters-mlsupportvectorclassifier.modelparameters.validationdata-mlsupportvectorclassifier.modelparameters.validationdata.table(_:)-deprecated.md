

- Create ML
- MLSupportVectorClassifier
- 
  - MLSupportVectorClassifier
- MLSupportVectorClassifier.ModelParameters
- MLSupportVectorClassifier.ModelParameters.ValidationData
-  MLSupportVectorClassifier.ModelParameters.ValidationData.table(\_:) Deprecated

Case

# MLSupportVectorClassifier.ModelParameters.ValidationData.table(\_:)

Set validation data from the MLDataTable provided.

macOS 10.15–14.0Deprecated

``` source
case table(MLDataTable)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generate validation data by splitting the training dataset. This is the default.

Deprecated

case dataFrame(DataFrame)

Validation data provided in a DataFrame.

Deprecated

case none

Do not set validation data.

Deprecated

