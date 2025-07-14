

- MusicKit
- MusicCatalogSearchResponse
-  MusicCatalogSearchResponse.TopResult 

Enumeration

# MusicCatalogSearchResponse.TopResult

An item that represents one of the top results in a catalog search response.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum TopResult
```

## Topics

### Operators

static func == (MusicCatalogSearchResponse.TopResult, MusicCatalogSearchResponse.TopResult) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case album(Album)

An item that corresponds to an album.

case artist(Artist)

An item that corresponds to an artist.

case curator(Curator)

An item that corresponds to a curator.

case musicVideo(MusicVideo)

An item that corresponds to a music video.

case playlist(Playlist)

An item that corresponds to a playlist.

case radioShow(RadioShow)

An item that corresponds to a radio show.

case recordLabel(RecordLabel)

An item that corresponds to a record label.

case song(Song)

An item that corresponds to a song.

case station(Station)

An item that corresponds to a station.

### Instance Properties

var artwork: Artwork?

The artwork of this top result for catalog search.

var hashValue: Int

The hash value.

var id: MusicItemID

The unique identifier of this top result for catalog search.

var title: String

The title of this top result for catalog search.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

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
- Identifiable
- MusicItem
- Sendable

