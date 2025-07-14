

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
- MLTextClassifier.ModelParameters.ValidationData
-  MLTextClassifier.ModelParameters.ValidationData.dataSource(\_:) 

Case

# MLTextClassifier.ModelParameters.ValidationData.dataSource(\_:)

Sets the validation data from the provided data source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case dataSource(MLTextClassifier.DataSource)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generates the validation data by splitting the training dataset.

case table(MLDataTable, textColumn: String, labelColumn: String)

Sets the validation data from the provided data table.

case dataFrame(DataFrame, textColumn: String, labelColumn: String)

Set validation data from the MLDataTable provided.

case dictionary([String : [String]])

Sets the validation data from the provided dictionary.

case none

Doesn’t set validation data.

