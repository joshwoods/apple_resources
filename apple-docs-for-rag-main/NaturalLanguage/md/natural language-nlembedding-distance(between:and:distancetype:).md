

- Natural Language
- NLEmbedding
-  distance(between:and:distanceType:) 

Instance Method

# distance(between:and:distanceType:)

Calculates the distance between two strings in the vocabulary space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@nonobjc
func distance(
    between firstString: String,
    and secondString: String,
    distanceType: NLDistanceType = .cosine
) -> NLDistance
```

## Parameters 

`firstString`  

A string in the embedding vocabulary.

`secondString`  

Another string in the embedding vocabulary.

`distanceType`  

A means of calculating distance that determines which formula the method uses to evaluate the distance between `firstString` and `secondString`.

## Return Value

The distance associated with `distanceType`.

## See Also

### Finding strings and their distances in an embedding

func neighbors(for: String, maximumCount: Int, distanceType: NLDistanceType) -> [(String, NLDistance)]

Retrieves a limited number of strings near a string in the vocabulary.

func neighbors(for: [Double], maximumCount: Int, distanceType: NLDistanceType) -> [(String, NLDistance)]

Retrieves a limited number of strings near a location in the vocabulary space.

func enumerateNeighbors(for: String, maximumCount: Int, distanceType: NLDistanceType, using: (String, NLDistance) -> Bool)

Passes the nearest strings of a string in the vocabulary to a closure.

func enumerateNeighbors(for: [Double], maximumCount: Int, distanceType: NLDistanceType, using: (String, NLDistance) -> Bool)

Passes the nearest strings of a location in the vocabulary space to a closure.

typealias NLDistance

The distance between two strings in a text embedding.

