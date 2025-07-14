

- Create ML
- MLWordTagger
-  prediction(from:) 

Instance Method

# prediction(from:)

Predicts a tag for the input string.

macOS 10.14+

``` source
func prediction(from text: String) throws -> [String]
```

## Parameters 

`text`  

The string to tag.

## Return Value

An array of tags for the tokens in the string.

## See Also

### Testing a word tagger

func predictions&lt;S>(from: S) throws -> DataFrame

Predicts sequences of labels, token locations, and token lengths from the input strings.

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataTable

Predicts sequences of labels, token locations, and token lengths from the input column containing strings.

Deprecated

func prediction(from: [MLWordTagger.Token]) throws -> [String]

Predicts a tag for each token in the specified array.

func predictionWithConfidence(from: String) throws -> [[String : Double]]

Predicts tags and confidence scores for the input string. Predicts tags and confidence scores for the input string.

func predictionWithConfidence(from: [MLWordTagger.Token]) throws -> [[String : Double]]

Predicts tags and confidence scores for each token in the specified token array.

