

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
- MLTextClassifier.ModelParameters.ValidationData
-  MLTextClassifier.ModelParameters.ValidationData.table(\_:textColumn:labelColumn:) 

Case

# MLTextClassifier.ModelParameters.ValidationData.table(\_:textColumn:labelColumn:)

Sets the validation data from the provided data table.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 10.15–14.0DeprecatedvisionOS 1.0+

``` source
case table(
    MLDataTable,
    textColumn: String,
    labelColumn: String
)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generates the validation data by splitting the training dataset.

case dataFrame(DataFrame, textColumn: String, labelColumn: String)

Set validation data from the MLDataTable provided.

case dataSource(MLTextClassifier.DataSource)

Sets the validation data from the provided data source.

case dictionary([String : [String]])

Sets the validation data from the provided dictionary.

case none

Doesn’t set validation data.

