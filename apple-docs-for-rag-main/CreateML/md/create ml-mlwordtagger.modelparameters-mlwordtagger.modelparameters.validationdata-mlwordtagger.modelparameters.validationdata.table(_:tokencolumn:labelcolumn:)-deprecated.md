

- Create ML
- MLWordTagger
- 
  - MLWordTagger
- MLWordTagger.ModelParameters
- MLWordTagger.ModelParameters.ValidationData
-  MLWordTagger.ModelParameters.ValidationData.table(\_:tokenColumn:labelColumn:) Deprecated

Case

# MLWordTagger.ModelParameters.ValidationData.table(\_:tokenColumn:labelColumn:)

Sets the validation data from the provided data table.

macOS 10.15–14.0Deprecated

``` source
case table(
    MLDataTable,
    tokenColumn: String,
    labelColumn: String
)
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generates the validation data by splitting the training dataset.

case dataFrame(DataFrame, tokenColumn: String, labelColumn: String)

Set validation data from the DataFrame provided.

case tuples([(tokens: [MLWordTagger.Token], labels: [String])])

Sets the validation data from a list of tokens and labels.

case none

Doesn’t set validation data.

