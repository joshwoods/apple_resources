

- Create ML
- MLTextClassifier
-  predictionWithConfidence(from:) 

Instance Method

# predictionWithConfidence(from:)

Predicts multiple possible labels and their confidence scores for the specified string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
func predictionWithConfidence(from text: String) throws -> [String : Double]
```

## Parameters 

`text`  

The string to classify.

## Return Value

A dictionary of label predictions and confidence scores.

## See Also

### Testing a text classifier

func prediction(from: String) throws -> String

Classifies a string with a label.

func predictions(from: [String]) throws -> [String]

Classifies an array of strings with labels.

func predictionsWithConfidence(from: [String]) throws -> [[String : Double]]

Predicts multiple possible labels and their confidence scores for each string in the specified array.

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;String>

Classifies a data column with labels.

Deprecated

func predictionsWithConfidence(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;[String : Double]>

Predicts multiple possible labels and their confidence scores for each string in the specified data column.

Deprecated

