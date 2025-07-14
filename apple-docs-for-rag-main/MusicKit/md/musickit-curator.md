

- MusicKit
-  Curator 

Structure

# Curator

A music item that represents a curator.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 9.0+

``` source
struct Curator
```

## Topics

### Operators

static func == (Curator, Curator) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var artwork: Artwork?

The curator artwork.

var editorialNotes: EditorialNotes?

The notes about the curator that appear in the Music catalog.

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the curator.

var kind: Curator.Kind

The kind of curator.

var name: String

The name of the curator.

var playlists: MusicItemCollection&lt;Playlist>?

The curator’s associated playlists.

var url: URL?

The URL for the curator.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Enumerations

enum Kind

The available kinds of curators.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

FilterableMusicItem Implementations

MusicItem Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- FilterableMusicItem
- Hashable
- Identifiable
- MusicCatalogSearchable
- MusicItem
- MusicPropertyContainer
- Sendable

## See Also

### Music Items

struct Album

A music item that represents an album.

struct Artist

A music item that represents an artist.

struct Genre

A music item that represents a genre.

struct MusicVideo

A music item that represents a music video.

struct Playlist

A music item that represents a playlist.

struct RadioShow

A music item that represents a radio show.

struct RecordLabel

A music item that represents a record label.

struct Song

A music item that represents a song.

struct Station

A music item that represents a station.

enum Track

A music item that represents a track.

