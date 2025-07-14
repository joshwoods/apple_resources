

- Natural Language
-  NLDistance 

Type Alias

# NLDistance

The distance between two strings in a text embedding.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
typealias NLDistance = Double
```

## Discussion

The meaning of an NLDistance is directly related to the NLDistanceType you use when you call a method that uses it. For example, if you use the neighborsForString:maximumCount:distanceType: method and use NLDistanceType.cosine for the `distanceType` parameter, the method calculates the cosine distance and returns it as an NLDistance.

## Topics

### Calculating Distance

enum NLDistanceType

The means of calculating a distance between two locations in a text embedding.

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

func distance(between: String, and: String, distanceType: NLDistanceType) -> NLDistance

Calculates the distance between two strings in the vocabulary space.

