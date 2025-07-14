

- MusicKit
-  MusicPersonalRecommendationsResponse 

Structure

# MusicPersonalRecommendationsResponse

An object that contains results for a personal recommendations request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicPersonalRecommendationsResponse
```

## Topics

### Operators

static func == (MusicPersonalRecommendationsResponse, MusicPersonalRecommendationsResponse) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let recommendations: MusicItemCollection&lt;MusicPersonalRecommendation>

A collection of personal recommendations.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

