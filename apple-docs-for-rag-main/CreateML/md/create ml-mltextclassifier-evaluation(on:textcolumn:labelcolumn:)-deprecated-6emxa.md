

- Create ML
- MLTextClassifier
-  evaluation(on:textColumn:labelColumn:) Deprecated

Instance Method

# evaluation(on:textColumn:labelColumn:)

Computes evaluation metrics.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–13.0DeprecatedvisionOS 1.0+

``` source
func evaluation(
    on labeledTexts: MLDataTable,
    textColumn: String,
    labelColumn: String
) -> MLClassifierMetrics
```

Deprecated

Use DataFrame instead of MLDataTable.

## Parameters 

`labeledTexts`  

The data table for the data to be evaluated

`textColumn`  

Name of the text column in the provided trainingData

`labelColumn`  

Name of the label column in the provided trainingData

## Return Value

A `MLClassifierMetrics` struct containing the computed metrics or an error message.

## See Also

### Evaluating a text classifier

func evaluation(on: MLTextClassifier.DataSource) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: DataFrame, textColumn: String, labelColumn: String) -> MLClassifierMetrics

Computes evaluation metrics.

func evaluation(on: [String : [String]]) -> MLClassifierMetrics

Computes evaluation metrics.

