

- Create ML
- MLTextClassifier
-  prediction(from:) 

Instance Method

# prediction(from:)

Classifies a string with a label.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
func prediction(from text: String) throws -> String
```

## Parameters 

`text`  

The string to be classified.

## Return Value

The label for the given string.

## See Also

### Testing a text classifier

func predictions(from: [String]) throws -> [String]

Classifies an array of strings with labels.

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

