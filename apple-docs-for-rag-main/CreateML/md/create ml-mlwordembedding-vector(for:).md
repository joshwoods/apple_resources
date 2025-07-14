

- Create ML
- MLWordEmbedding
-  vector(for:) 

Instance Method

# vector(for:)

Accesses the vector associated with the given string in the vocabulary.

macOS 10.15+

``` source
func vector(for text: String) -> [Double]?
```

## Parameters 

`text`  

A string in the vocabulary.

## Return Value

The vector associated with the string if present in the word embedding; otherwise, `nil`.

## See Also

### Testing a word embedding

func prediction(from: String, maxCount: Int, maxDistance: Double, distanceType: NLDistanceType) throws -> [(text: String, distance: Double)]

Predicts neighbors.

func distance(between: String, and: String, distanceType: NLDistanceType) -> Double

Calculates the distance between two strings in the vocabulary space.

enum NLDistanceType

The means of calculating a distance between two locations in a text embedding.

func contains(String) -> Bool

Returns a Boolean value indicating whether the vocabulary contains the given string.

