

- Create ML
- MLTextClassifier
-  evaluation(on:textColumn:labelColumn:) 

Instance Method

# evaluation(on:textColumn:labelColumn:)

Computes evaluation metrics.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func evaluation(
    on dataFrame: DataFrame,
    textColumn: String,
    labelColumn: String
) -> MLClassifierMetrics
```

## Parameters 

`dataFrame`  

A data frame containing labeled examples.

`textColumn`  

The name of the text column.

`labelColumn`  

The name of the label column.

## Return Value

The computed metrics or an error message.

## See Also

### Evaluating a text classifier

func evaluation(on: MLTextClassifier.DataSource) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: [String : [String]]) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: MLDataTable, textColumn: String, labelColumn: String) -> MLClassifierMetrics

Computes evaluation metrics.

Deprecated

