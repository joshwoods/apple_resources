

- MusicKit
-  Genre 

Structure

# Genre

A music item that represents a genre.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Genre
```

## Topics

### Operators

static func == (Genre, Genre) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the genre.

var libraryAddedDate: Date?

The date when the user added the genre to the library.

var name: String

The localized name of the genre.

var parent: Genre?

The parent genre, if any.

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

MusicLibraryRequestable Implementations

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
- MusicCatalogTopLevelResourceRequesting
- MusicItem
- MusicLibraryRequestable
- MusicLibrarySectionRequestable
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

