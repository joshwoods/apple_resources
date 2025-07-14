

- MusicKit
-  MusicCatalogSearchable 

Protocol

# MusicCatalogSearchable

A protocol for music items that your app can fetch by using a catalog search request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol MusicCatalogSearchable : MusicItem
```

## Relationships

### Inherits From

- MusicItem
- Sendable

### Conforming Types

- Album
- Artist
- Curator
- MusicVideo
- Playlist
- RadioShow
- RecordLabel
- Song
- Station

## See Also

### Catalog Search

struct MusicCatalogSearchRequest

A request that your app uses to fetch items from the Apple Music catalog using a search term.

struct MusicCatalogSearchResponse

An object that contains results for a catalog search request.

