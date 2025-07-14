

- Create ML
- MLWordTagger
- MLWordTagger.ModelParameters
- MLWordTagger.ModelParameters.ValidationData
-  MLWordTagger.ModelParameters.ValidationData.tuples(\_:) 

Case

# MLWordTagger.ModelParameters.ValidationData.tuples(\_:)

Sets the validation data from a list of tokens and labels.

macOS 10.15+

``` source
case tuples([(tokens: [MLWordTagger.Token], labels: [String])])
```

## See Also

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generates the validation data by splitting the training dataset.

case table(MLDataTable, tokenColumn: String, labelColumn: String)

Sets the validation data from the provided data table.

Deprecated

case dataFrame(DataFrame, tokenColumn: String, labelColumn: String)

Set validation data from the DataFrame provided.

case none

Doesn’t set validation data.

