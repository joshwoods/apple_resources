

- Create ML
- MLTextClassifier
-  predictionsWithConfidence(from:) Deprecated

Instance Method

# predictionsWithConfidence(from:)

Predicts multiple possible labels and their confidence scores for each string in the specified data column.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 11.0–13.0DeprecatedvisionOS 1.0+

``` source
func predictionsWithConfidence(from texts: MLDataColumn) throws -> MLDataColumn
```

Deprecated

Use DataFrame instead of MLDataTable.

## Parameters 

`texts`  

The data column of strings to classify.

## Return Value

A data column of dictionaries. Each dictionary corresponds to a string in the input data column. A dictionary entry contains a label prediction with its associated confidence score.

## See Also

### Testing a text classifier

func prediction(from: String) throws -> String

Classifies a string with a label.

func predictions(from: [String]) throws -> [String]

Classifies an array of strings with labels.

func predictionWithConfidence(from: String) throws -> [String : Double]

Predicts multiple possible labels and their confidence scores for the specified string.

func predictionsWithConfidence(from: [String]) throws -> [[String : Double]]

Predicts multiple possible labels and their confidence scores for each string in the specified array.

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;String>

Classifies a data column with labels.

Deprecated

