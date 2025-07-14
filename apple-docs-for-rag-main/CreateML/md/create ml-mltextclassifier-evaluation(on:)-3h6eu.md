

- Create ML
- MLTextClassifier
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Computes evaluation metrics.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func evaluation(on labeledTexts: [String : [String]]) -> MLClassifierMetrics
```

## Parameters 

`labeledTexts`  

A dictionary of labeled texts to evaluate.

## Return Value

Classifier metrics.

## See Also

### Evaluating a text classifier

func evaluation(on: MLTextClassifier.DataSource) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: DataFrame, textColumn: String, labelColumn: String) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: MLDataTable, textColumn: String, labelColumn: String) -> MLClassifierMetrics

Computes evaluation metrics.

Deprecated

