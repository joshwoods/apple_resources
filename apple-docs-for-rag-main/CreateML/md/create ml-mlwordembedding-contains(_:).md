

- Create ML
- MLWordEmbedding
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the vocabulary contains the given string.

macOS 10.15+

``` source
func contains(_ text: String) -> Bool
```

## Parameters 

`text`  

The string to find in the vocabulary.

## Return Value

`true` if the string was found in the vocabulary; otherwise, false.

## See Also

### Testing a word embedding

func prediction(from: String, maxCount: Int, maxDistance: Double, distanceType: NLDistanceType) throws -> [(text: String, distance: Double)]

Predicts neighbors.

func distance(between: String, and: String, distanceType: NLDistanceType) -> Double

Calculates the distance between two strings in the vocabulary space.

enum NLDistanceType

The means of calculating a distance between two locations in a text embedding.

func vector(for: String) -> [Double]?

Accesses the vector associated with the given string in the vocabulary.

