

- Create ML
- MLWordTagger
-  predictions(from:) 

Instance Method

# predictions(from:)

Predicts sequences of labels, token locations, and token lengths from the input strings.

macOS 13.0+

``` source
func predictions(from texts: S) throws -> DataFrame where S : Sequence, S.Element == String
```

## Parameters 

`texts`  

A sequence of strings to tokenize and tag.

## Return Value

A `DataFrame` containing predicted labels, token locations, and token lengths.

## See Also

### Testing a word tagger

func predictions(from: MLDataColumn&lt;String>) throws -> MLDataTable

Predicts sequences of labels, token locations, and token lengths from the input column containing strings.

Deprecated

func prediction(from: [MLWordTagger.Token]) throws -> [String]

Predicts a tag for each token in the specified array.

func prediction(from: String) throws -> [String]

Predicts a tag for the input string.

func predictionWithConfidence(from: String) throws -> [[String : Double]]

Predicts tags and confidence scores for the input string. Predicts tags and confidence scores for the input string.

func predictionWithConfidence(from: [MLWordTagger.Token]) throws -> [[String : Double]]

Predicts tags and confidence scores for each token in the specified token array.

