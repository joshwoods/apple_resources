

- Create ML
- MLWordTagger
-  evaluation(on:tokenColumn:labelColumn:) 

Instance Method

# evaluation(on:tokenColumn:labelColumn:)

Computes evaluation metrics.

macOS 13.0+

``` source
func evaluation(
    on labeledTokens: DataFrame,
    tokenColumn: String,
    labelColumn: String
) -> MLWordTaggerMetrics
```

## Parameters 

`labeledTokens`  

An data frame containing tokens and labels.

`tokenColumn`  

The name of the token column in the data frame.

`labelColumn`  

The name of the label column in the data frame.

## Return Value

Word tagger metrics.

## See Also

### Evaluating a word tagger

func evaluation(on: MLDataTable, tokenColumn: String, labelColumn: String) -> MLWordTaggerMetrics

Computes evaluation metrics.

Deprecated

func evaluation(on: [(tokens: [MLWordTagger.Token], labels: [String])]) -> MLWordTaggerMetrics

Computes evaluation metrics.

