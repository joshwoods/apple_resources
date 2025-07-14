

- MusicKit
-  MusicCatalogChartsRequest 

Structure

# MusicCatalogChartsRequest

A request that your app uses to fetch the most popular items in the Apple Music catalog.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicCatalogChartsRequest
```

## Topics

### Operators

static func == (MusicCatalogChartsRequest, MusicCatalogChartsRequest) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(genre: Genre?, kinds: [MusicCatalogChartKind], types: [any MusicCatalogChartRequestable.Type])

Creates a catalog charts request for a specified genre and list of types to include in the catalog charts response.

### Instance Properties

var genre: Genre?

The genre for the request.

var hashValue: Int

The hash value.

var kinds: [MusicCatalogChartKind]

The kinds of requested catalog charts.

var limit: Int?

A limit for the number of items to return in the catalog search response.

var offset: Int?

An offet for the request.

var types: [any MusicCatalogChartRequestable.Type]

The list of requested types for the catalog charts response.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

func response() async throws -> MusicCatalogChartsResponse

Fetches the most popular items of the requested types that match the genre and kinds for the request.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

