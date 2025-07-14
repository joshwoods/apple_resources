

- Create ML
- MLWordTagger
- MLWordTagger.ModelParameters
- MLWordTagger.ModelParameters.ValidationData
-  MLWordTagger.ModelParameters.ValidationData.dataFrame(\_:tokenColumn:labelColumn:) 

Case

# MLWordTagger.ModelParameters.ValidationData.dataFrame(\_:tokenColumn:labelColumn:)

Set validation data from the DataFrame provided.

macOS 13.0+

``` source
case dataFrame(
    DataFrame,
    tokenColumn: String,
    labelColumn: String
)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generates the validation data by splitting the training dataset.

case table(MLDataTable, tokenColumn: String, labelColumn: String)

Sets the validation data from the provided data table.

Deprecated

case tuples([(tokens: [MLWordTagger.Token], labels: [String])])

Sets the validation data from a list of tokens and labels.

case none

Doesn’t set validation data.

