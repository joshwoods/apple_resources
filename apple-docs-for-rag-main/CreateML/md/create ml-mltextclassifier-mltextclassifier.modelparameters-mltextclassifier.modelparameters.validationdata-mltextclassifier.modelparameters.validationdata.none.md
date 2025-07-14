

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
- MLTextClassifier.ModelParameters.ValidationData
-  MLTextClassifier.ModelParameters.ValidationData.none 

Case

# MLTextClassifier.ModelParameters.ValidationData.none

Doesn’t set validation data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case none
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generates the validation data by splitting the training dataset.

case table(MLDataTable, textColumn: String, labelColumn: String)

Sets the validation data from the provided data table.

case dataFrame(DataFrame, textColumn: String, labelColumn: String)

Set validation data from the MLDataTable provided.

case dataSource(MLTextClassifier.DataSource)

Sets the validation data from the provided data source.

case dictionary([String : [String]])

Sets the validation data from the provided dictionary.

