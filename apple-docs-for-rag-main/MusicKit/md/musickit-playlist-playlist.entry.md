

- MusicKit
- Playlist
-  Playlist.Entry 

Structure

# Playlist.Entry

A music item that represents a playlist entry.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Entry
```

## Topics

### Operators

static func == (Playlist.Entry, Playlist.Entry) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var albumTitle: String?

The title of the album the playlist entry appears on.

var artistName: String

The artist’s name.

var artistURL: URL?

The artist’s URL.

var artwork: Artwork?

The artwork of the playlist entry.

var contentRating: ContentRating?

The rating of the content.

var duration: TimeInterval?

The duration of the playlist entry.

var editorialNotes: EditorialNotes?

The editorial notes for the playlist entry.

var genreNames: [String]

The names of the playlist entry’s associated genres.

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the playlist entry.

var isrc: String?

The International Standard Recording Code (ISRC) for the playlist entry.

var item: Playlist.Entry.Item?

The item of the playlist entry.

var lastPlayedDate: Date?

The date when the user last played the playlist entry on this device.

var libraryAddedDate: Date?

The date when the user added the playlist entry to the library.

var playCount: Int?

The number of times the user played the playlist entry.

var playParameters: PlayParameters?

The parameters to use to play the playlist entry.

var position: Int

The position of the playlist entry.

var previewAssets: [PreviewAsset]?

The preview assets for the playlist entry.

var releaseDate: Date?

The release date (or expected for pre-release) of the playlist entry.

var title: String

The title of the playlist entry.

var url: URL?

The URL for the playlist entry.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Enumerations

enum Item

An item that corresponds to an entry in a playlist.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

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
- Hashable
- Identifiable
- MusicItem
- MusicLibraryAddable
- MusicLibraryRequestable
- MusicPlaylistAddable
- MusicPropertyContainer
- PlayableMusicItem
- Sendable

