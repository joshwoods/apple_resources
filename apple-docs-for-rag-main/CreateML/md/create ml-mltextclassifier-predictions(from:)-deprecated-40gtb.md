

- Create ML
- MLTextClassifier
-  predictions(from:) Deprecated

Instance Method

# predictions(from:)

Classifies a data column with labels.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–13.0DeprecatedvisionOS 1.0+

``` source
func predictions(from texts: MLDataColumn) throws -> MLDataColumn
```

Deprecated

Use DataSource instead of MLDataTable.

## Parameters 

`texts`  

The data column of strings to be classified.

## Return Value

An array of labels for the given strings.

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

func predictionsWithConfidence(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;[String : Double]>

Predicts multiple possible labels and their confidence scores for each string in the specified data column.

Deprecated

