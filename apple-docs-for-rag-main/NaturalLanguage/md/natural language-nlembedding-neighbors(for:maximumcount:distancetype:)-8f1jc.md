

- Natural Language
- NLEmbedding
-  neighbors(for:maximumCount:distanceType:) 

Instance Method

# neighbors(for:maximumCount:distanceType:)

Retrieves a limited number of strings near a string in the vocabulary.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@nonobjc
func neighbors(
    for string: String,
    maximumCount maxCount: Int,
    distanceType: NLDistanceType = .cosine
) -> [(String, NLDistance)]
```

## Parameters 

`string`  

A string in the embedding vocabulary.

`maxCount`  

The largest number of neighboring strings that the method can return in an array.

`distanceType`  

A means of calculating distance that determines which formula the method uses to evaluate a neighbor’s distance from `string`.

## Return Value

An array of tuples that contain neighboring strings and their distances.

## See Also

### Finding strings and their distances in an embedding

func neighbors(for: [Double], maximumCount: Int, distanceType: NLDistanceType) -> [(String, NLDistance)]

Retrieves a limited number of strings near a location in the vocabulary space.

func enumerateNeighbors(for: String, maximumCount: Int, distanceType: NLDistanceType, using: (String, NLDistance) -> Bool)

Passes the nearest strings of a string in the vocabulary to a closure.

func enumerateNeighbors(for: [Double], maximumCount: Int, distanceType: NLDistanceType, using: (String, NLDistance) -> Bool)

Passes the nearest strings of a location in the vocabulary space to a closure.

func distance(between: String, and: String, distanceType: NLDistanceType) -> NLDistance

Calculates the distance between two strings in the vocabulary space.

typealias NLDistance

The distance between two strings in a text embedding.

