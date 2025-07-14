

- Create ML
- MLWordEmbedding
-  distance(between:and:distanceType:) 

Instance Method

# distance(between:and:distanceType:)

Calculates the distance between two strings in the vocabulary space.

macOS 10.15+

``` source
func distance(
    between first: String,
    and second: String,
    distanceType: NLDistanceType = .cosine
) -> Double
```

## Parameters 

`first`  

A string in the embedding vocabulary.

`second`  

Another string in the embedding vocabulary.

`distanceType`  

The metric to use to calculate the distance between the first and second strings.

## Return Value

The distance

## See Also

### Testing a word embedding

func prediction(from: String, maxCount: Int, maxDistance: Double, distanceType: NLDistanceType) throws -> [(text: String, distance: Double)]

Predicts neighbors.

enum NLDistanceType

The means of calculating a distance between two locations in a text embedding.

func contains(String) -> Bool

Returns a Boolean value indicating whether the vocabulary contains the given string.

func vector(for: String) -> [Double]?

Accesses the vector associated with the given string in the vocabulary.

