

- MusicKit
-  MusicPersonalRecommendationsRequest 

Structure

# MusicPersonalRecommendationsRequest

A request that your app uses to fetch music recommendations based on the user’s library and listening history.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicPersonalRecommendationsRequest
```

## Topics

### Operators

static func == (MusicPersonalRecommendationsRequest, MusicPersonalRecommendationsRequest) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

Creates a request to fetch default personal recommendations for the user.

init&lt;S>(refreshing: S)

Creates a request to fetch default personal recommendations for the user.

### Instance Properties

var hashValue: Int

The hash value.

var limit: Int?

A limit for the number of recommendations to return in the personal recommendations response.

var offset: Int?

An offet for the request.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

func response() async throws -> MusicPersonalRecommendationsResponse

Fetches the music recommendations based on the user’s library and listening history.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

