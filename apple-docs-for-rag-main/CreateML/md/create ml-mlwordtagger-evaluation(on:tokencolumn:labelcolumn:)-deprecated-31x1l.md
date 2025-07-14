

- Create ML
- MLWordTagger
-  evaluation(on:tokenColumn:labelColumn:) Deprecated

Instance Method

# evaluation(on:tokenColumn:labelColumn:)

Computes evaluation metrics.

macOS 10.14–13.0Deprecated

``` source
func evaluation(
    on labeledTokens: MLDataTable,
    tokenColumn: String,
    labelColumn: String
) -> MLWordTaggerMetrics
```

## Parameters 

`labeledTokens`  

A table containing tokens and labels.

`tokenColumn`  

The name of the token column in the data frame.

`labelColumn`  

The name of the label column in the data frame.

## Return Value

Word tagger metrics.

## See Also

### Evaluating a word tagger

func evaluation(on: DataFrame, tokenColumn: String, labelColumn: String) -> MLWordTaggerMetrics

Computes evaluation metrics.

func evaluation(on: [(tokens: [MLWordTagger.Token], labels: [String])]) -> MLWordTaggerMetrics

Computes evaluation metrics.

