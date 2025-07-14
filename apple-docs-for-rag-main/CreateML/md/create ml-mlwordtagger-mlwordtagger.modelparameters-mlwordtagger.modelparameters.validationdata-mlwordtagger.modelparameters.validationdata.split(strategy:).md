

- Create ML
- MLWordTagger
- MLWordTagger.ModelParameters
- MLWordTagger.ModelParameters.ValidationData
-  MLWordTagger.ModelParameters.ValidationData.split(strategy:) 

Case

# MLWordTagger.ModelParameters.ValidationData.split(strategy:)

Generates the validation data by splitting the training dataset.

macOS 10.15+

``` source
case split(strategy: MLSplitStrategy)
```

## Discussion

By default, model parameters use this approach to specify the validation data.

## See Also

### Specifying validation data

case table(MLDataTable, tokenColumn: String, labelColumn: String)

Sets the validation data from the provided data table.

Deprecated

case dataFrame(DataFrame, tokenColumn: String, labelColumn: String)

Set validation data from the DataFrame provided.

case tuples([(tokens: [MLWordTagger.Token], labels: [String])])

Sets the validation data from a list of tokens and labels.

case none

Doesn’t set validation data.

