

- MusicKit
-  MusicItem 

Protocol

# MusicItem

A protocol with basic requirements for music items.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol MusicItem : Sendable
```

## Topics

### Instance Properties

var id: MusicItemID

The unique identifier for the music item.

**Required**

### Instance Methods

func with([PartialMusicAsyncProperty&lt;Self>]) async throws -> Self

Loads a new instance of the music item that includes the specified properties.

func with(PartialMusicAsyncProperty&lt;Self>..., preferredSource: MusicPropertySource) async throws -> Self

Loads a new instance of the music item that includes the specified properties.

func with([PartialMusicAsyncProperty&lt;Self>], preferredSource: MusicPropertySource) async throws -> Self

Loads a new instance of the music item that includes the specified properties.

## Relationships

### Inherits From

- Sendable

### Inherited By

- FilterableMusicItem
- MusicCatalogChartRequestable
- MusicCatalogSearchable
- MusicCatalogTopLevelResourceRequesting
- MusicLibraryAddable
- MusicLibraryRequestable
- MusicLibrarySearchable
- MusicPersonalRecommendationItem
- MusicPlaylistAddable
- MusicRecentlyPlayedRequestable
- PlayableMusicItem

### Conforming Types

- Album
- Artist
- Curator
- Genre
- MusicCatalogSearchResponse.TopResult
- MusicLibrarySearchResponse.TopResult
- MusicPersonalRecommendation
- MusicPersonalRecommendation.Item
- MusicPlayer.Queue.Entry.Item
- MusicVideo
- Playlist
- Playlist.Entry
- Playlist.Entry.Item
- RadioShow
- RecentlyPlayedMusicItem
- RecordLabel
- Song
- Station
- Track

## See Also

### Utility

struct MusicItemID

An object that represents a unique identifier for a music item.

struct MusicItemCollection

A collection of music items.

protocol MusicPropertyContainer

A protocol for music items that allow loading additional properties that you can fetch asynchronously.

class MusicRelationshipProperty

An identifier for a music item relationship property from a specific root type to a specific value type for the element of the resulting collection.

class MusicExtendedAttributeProperty

An identifier for a music item extended attribute property from a specific root type to a specific resulting value type.

class MusicAttributeProperty

An identifier for a music item attribute property from a specific root type to a specific resulting value type.

class PartialMusicAsyncProperty

A partially type-erased identifier for a music item property that you can fetch asynchronously from a concrete root type to any resulting value type.

class PartialMusicProperty

A partially type-erased identifier for a music item property from a concrete root type to any resulting value type.

class AnyMusicProperty

A type-erased identifier for a music item property, from any root type to any resulting value type.

