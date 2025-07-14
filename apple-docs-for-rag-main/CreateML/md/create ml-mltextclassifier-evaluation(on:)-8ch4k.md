

- Create ML
- MLTextClassifier
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Computes evaluation metrics.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func evaluation(on labeledTexts: MLTextClassifier.DataSource) -> MLClassifierMetrics
```

## Parameters 

`labeledTexts`  

A data source of labeled texts to evaluate.

## Return Value

Classifier metrics.

## Mentioned in 

Creating a Text Classifier Model

Creating a text classifier model

## See Also

### Evaluating a text classifier

func evaluation(on: DataFrame, textColumn: String, labelColumn: String) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: [String : [String]]) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: MLDataTable, textColumn: String, labelColumn: String) -> MLClassifierMetrics

Computes evaluation metrics.

Deprecated

