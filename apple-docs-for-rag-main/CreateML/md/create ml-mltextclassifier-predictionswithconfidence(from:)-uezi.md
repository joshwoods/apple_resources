

- Create ML
- MLTextClassifier
-  predictionsWithConfidence(from:) 

Instance Method

# predictionsWithConfidence(from:)

Predicts multiple possible labels and their confidence scores for each string in the specified array.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
func predictionsWithConfidence(from texts: [String]) throws -> [[String : Double]]
```

## Parameters 

`texts`  

The array of strings to classify.

## Return Value

An array of dictionaries. Each dictionary corresponds to a string in the input array. A dictionary entry contains a label prediction with its associated confidence score.

## See Also

### Testing a text classifier

func prediction(from: String) throws -> String

Classifies a string with a label.

func predictions(from: [String]) throws -> [String]

Classifies an array of strings with labels.

func predictionWithConfidence(from: String) throws -> [String : Double]

Predicts multiple possible labels and their confidence scores for the specified string.

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;String>

Classifies a data column with labels.

Deprecated

func predictionsWithConfidence(from: MLDataColumn&lt;String>) throws -> MLDataColumn&lt;[String : Double]>

Predicts multiple possible labels and their confidence scores for each string in the specified data column.

Deprecated

