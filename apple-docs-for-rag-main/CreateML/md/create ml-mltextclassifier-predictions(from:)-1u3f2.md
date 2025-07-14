

- Create ML
- MLTextClassifier
-  predictions(from:) 

Instance Method

# predictions(from:)

Classifies an array of strings with labels.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func predictions(from texts: [String]) throws -> [String]
```

## Parameters 

`texts`  

The array of strings to be classified.

## Return Value

An array of labels for the given strings.

## See Also

### Testing a text classifier

func prediction(from: String) throws -> String

Classifies a string with a label.

func predictionWithConfidence(from: String) throws -> [String : Double]

Predicts multiple possible labels and their confidence scores for the specified string.

func predictionsWithConfidence(from: [String]) throws -> [[String : Double]]

Predicts multiple possible labels and their confidence scores for each string in the specified array.

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;String>

Classifies a data column with labels.

Deprecated

func predictionsWithConfidence(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;[String : Double]>

Predicts multiple possible labels and their confidence scores for each string in the specified data column.

Deprecated

