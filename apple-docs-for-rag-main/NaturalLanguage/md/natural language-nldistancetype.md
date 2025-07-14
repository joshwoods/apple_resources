

- Natural Language
-  NLDistanceType 

Enumeration

# NLDistanceType

The means of calculating a distance between two locations in a text embedding.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum NLDistanceType
```

## Overview

The meaning of an NLDistance is directly related to the NLDistanceType you use when you call a method that uses it. For example, if you use the neighborsForString:maximumCount:distanceType: method and use NLDistanceType.cosine for the `distanceType` parameter, the method calculates the cosine distance and returns it as an NLDistance.

## Topics

### Distance Types

case cosine

A method of calculating distance by using cosine similarity.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

