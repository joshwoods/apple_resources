

- Natural Language
- NLEmbedding
-  enumerateNeighbors(for:maximumCount:distanceType:using:) 

Instance Method

# enumerateNeighbors(for:maximumCount:distanceType:using:)

Passes the nearest strings of a location in the vocabulary space to a closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@nonobjc
func enumerateNeighbors(
    for vector: [Double],
    maximumCount maxCount: Int,
    distanceType: NLDistanceType = .cosine,
    using block: (String, NLDistance) -> Bool
)
```

## Parameters 

`vector`  

A location in the vocabulary space.

`maxCount`  

The largest number of times the method calls `block`.

`distanceType`  

A means of calculating distance that determines which formula the method uses to evaluate a neighbor’s distance from `vector`.

`block`  

A closure with the following parameters:

`String`  
A neighboring string.

`NLDistance`  
The distance from `vector` to the neighboring string.

The closure returns a Boolean that indicates whether to stop enumerating neighbors.

## See Also

### Finding strings and their distances in an embedding

func neighbors(for: String, maximumCount: Int, distanceType: NLDistanceType) -> [(String, NLDistance)]

Retrieves a limited number of strings near a string in the vocabulary.

func neighbors(for: [Double], maximumCount: Int, distanceType: NLDistanceType) -> [(String, NLDistance)]

Retrieves a limited number of strings near a location in the vocabulary space.

func enumerateNeighbors(for: String, maximumCount: Int, distanceType: NLDistanceType, using: (String, NLDistance) -> Bool)

Passes the nearest strings of a string in the vocabulary to a closure.

func distance(between: String, and: String, distanceType: NLDistanceType) -> NLDistance

Calculates the distance between two strings in the vocabulary space.

typealias NLDistance

The distance between two strings in a text embedding.

