

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
- MLTextClassifier.ModelParameters.ValidationData
-  MLTextClassifier.ModelParameters.ValidationData.dataFrame(\_:textColumn:labelColumn:) 

Case

# MLTextClassifier.ModelParameters.ValidationData.dataFrame(\_:textColumn:labelColumn:)

Set validation data from the MLDataTable provided.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
case dataFrame(
    DataFrame,
    textColumn: String,
    labelColumn: String
)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generates the validation data by splitting the training dataset.

case table(MLDataTable, textColumn: String, labelColumn: String)

Sets the validation data from the provided data table.

case dataSource(MLTextClassifier.DataSource)

Sets the validation data from the provided data source.

case dictionary([String : [String]])

Sets the validation data from the provided dictionary.

case none

Doesn’t set validation data.

