

- Create ML
- MLSupportVectorClassifier
- 
  - MLSupportVectorClassifier
- MLSupportVectorClassifier.ModelParameters
- MLSupportVectorClassifier.ModelParameters.ValidationData
-  MLSupportVectorClassifier.ModelParameters.ValidationData.dataFrame(\_:) Deprecated

Case

# MLSupportVectorClassifier.ModelParameters.ValidationData.dataFrame(\_:)

Validation data provided in a DataFrame.

macOS 12.0–14.0Deprecated

``` source
case dataFrame(DataFrame)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generate validation data by splitting the training dataset. This is the default.

Deprecated

case table(MLDataTable)

Set validation data from the MLDataTable provided.

Deprecated

case none

Do not set validation data.

Deprecated

