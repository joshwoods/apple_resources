

- Create ML
- MLWordTagger
-  predictionWithConfidence(from:) 

Instance Method

# predictionWithConfidence(from:)

Predicts tags and confidence scores for the input string. Predicts tags and confidence scores for the input string.

macOS 11.0+

``` source
func predictionWithConfidence(from text: String) throws -> [[String : Double]]
```

## Parameters 

`text`  

The string to tag.

## Return Value

An array of dictionaries. Each dictionary corresponds to a token in the input text string. A dictionary entry contains a tag prediction with its associated confidence score.

## See Also

### Testing a word tagger

func predictions&lt;S>(from: S) throws -> DataFrame

Predicts sequences of labels, token locations, and token lengths from the input strings.

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataTable

Predicts sequences of labels, token locations, and token lengths from the input column containing strings.

Deprecated

func prediction(from: [MLWordTagger.Token]) throws -> [String]

Predicts a tag for each token in the specified array.

func prediction(from: String) throws -> [String]

Predicts a tag for the input string.

func predictionWithConfidence(from: [MLWordTagger.Token]) throws -> [[String : Double]]

Predicts tags and confidence scores for each token in the specified token array.

