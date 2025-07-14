

- Create ML
- MLWordTagger
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Computes evaluation metrics.

macOS 10.14+

``` source
func evaluation(on labeledTokens: [(tokens: [MLWordTagger.Token], labels: [String])]) -> MLWordTaggerMetrics
```

## Parameters 

`labeledTokens`  

An array of token and label pairs.

## Return Value

Word tagger metrics.

## See Also

### Evaluating a word tagger

func evaluation(on: MLDataTable, tokenColumn: String, labelColumn: String) -> MLWordTaggerMetrics

Computes evaluation metrics.

Deprecated

func evaluation(on: DataFrame, tokenColumn: String, labelColumn: String) -> MLWordTaggerMetrics

Computes evaluation metrics.

