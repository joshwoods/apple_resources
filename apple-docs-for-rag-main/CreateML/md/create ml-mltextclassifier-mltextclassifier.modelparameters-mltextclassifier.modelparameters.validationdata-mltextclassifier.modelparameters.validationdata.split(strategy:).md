

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
- MLTextClassifier.ModelParameters.ValidationData
-  MLTextClassifier.ModelParameters.ValidationData.split(strategy:) 

Case

# MLTextClassifier.ModelParameters.ValidationData.split(strategy:)

Generates the validation data by splitting the training dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
case split(strategy: MLSplitStrategy)
```

## Discussion

By default, model parameters use this approach to specify the validation data.

## See Also

### Specifying validation data

case table(MLDataTable, textColumn: String, labelColumn: String)

Sets the validation data from the provided data table.

case dataFrame(DataFrame, textColumn: String, labelColumn: String)

Set validation data from the MLDataTable provided.

case dataSource(MLTextClassifier.DataSource)

Sets the validation data from the provided data source.

case dictionary([String : [String]])

Sets the validation data from the provided dictionary.

case none

Doesn’t set validation data.

