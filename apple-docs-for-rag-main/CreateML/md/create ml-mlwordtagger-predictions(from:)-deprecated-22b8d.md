

- Create ML
- MLWordTagger
-  predictions(from:) Deprecated

Instance Method

# predictions(from:)

Predicts sequences of labels, token locations, and token lengths from the input column containing strings.

macOS 10.14–13.0Deprecated

``` source
func predictions(from texts: MLDataColumn) throws -> MLDataTable
```

## Parameters 

`texts`  

A column of strings to tokenize and tag.

## Return Value

A table containing predicted labels, token locations, and token lengths.

## See Also

### Testing a word tagger

func predictions&lt;S>(from: S) throws -> DataFrame

Predicts sequences of labels, token locations, and token lengths from the input strings.

func prediction(from: [MLWordTagger.Token]) throws -> [String]

Predicts a tag for each token in the specified array.

func prediction(from: String) throws -> [String]

Predicts a tag for the input string.

func predictionWithConfidence(from: String) throws -> [[String : Double]]

Predicts tags and confidence scores for the input string. Predicts tags and confidence scores for the input string.

func predictionWithConfidence(from: [MLWordTagger.Token]) throws -> [[String : Double]]

Predicts tags and confidence scores for each token in the specified token array.

