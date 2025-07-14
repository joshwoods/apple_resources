

- MusicKit
-  RadioShow 

Structure

# RadioShow

A music item that represents a radio show.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 9.0+

``` source
struct RadioShow
```

## Topics

### Operators

static func == (RadioShow, RadioShow) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var artwork: Artwork?

The radio show artwork.

var editorialNotes: EditorialNotes?

The notes about the radio show that appear in the Music catalog.

var hashValue: Int

The hash value.

var hostName: String?

The name of the host for the radio show.

let id: MusicItemID

The unique identifier for the radio show.

var name: String

The name of the radio show.

var playlists: MusicItemCollection&lt;Playlist>?

The radio show’s associated playlists.

var url: URL?

The URL for the radio show.

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

struct Curator

A music item that represents a curator.

struct Genre

A music item that represents a genre.

struct MusicVideo

A music item that represents a music video.

struct Playlist

A music item that represents a playlist.

struct RecordLabel

A music item that represents a record label.

struct Song

A music item that represents a song.

struct Station

A music item that represents a station.

enum Track

A music item that represents a track.

