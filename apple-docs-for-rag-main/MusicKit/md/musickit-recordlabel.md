

- MusicKit
-  RecordLabel 

Structure

# RecordLabel

A music item that represents a record label.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct RecordLabel
```

## Topics

### Operators

static func == (RecordLabel, RecordLabel) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var artwork: Artwork?

The record label’s artwork.

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the record label.

var latestReleases: MusicItemCollection&lt;Album>?

A collection of the most recent releases for the record label.

var name: String

The name of the record label.

var shortDescription: String?

An abbreviated description to show inline or when the record label appears alongside other content.

var standardDescription: String?

A description to show when the record label is prominently displayed.

var topReleases: MusicItemCollection&lt;Album>?

A collection of top releases for the record label.

var url: URL?

The URL for the record label.

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

struct RadioShow

A music item that represents a radio show.

struct Song

A music item that represents a song.

struct Station

A music item that represents a station.

enum Track

A music item that represents a track.

