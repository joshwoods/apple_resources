

- MusicKit
- Playlist
- Playlist.Entry
-  Playlist.Entry.Item 

Enumeration

# Playlist.Entry.Item

An item that corresponds to an entry in a playlist.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Item
```

## Topics

### Operators

static func == (Playlist.Entry.Item, Playlist.Entry.Item) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case musicVideo(MusicVideo)

An item that corresponds to a music video.

case song(Song)

An item that corresponds to a song.

### Instance Properties

var albumTitle: String?

The title of the album the playlist entry’s item appears on.

var artistName: String

The artist’s name.

var artistURL: URL?

The artist’s URL.

var artwork: Artwork?

The artwork for the playlist entry’s item.

var contentRating: ContentRating?

The rating of the content.

var duration: TimeInterval?

The duration of the playlist entry’s item.

var editorialNotes: EditorialNotes?

The editorial notes for the playlist entry’s item.

var genreNames: [String]

The names of the playlist entry’s item associated genres.

var hashValue: Int

The hash value.

var id: MusicItemID

The unique identifier for the playlist entry item.

var isrc: String?

The International Standard Recording Code (ISRC) for the playlist entry’s item.

var lastPlayedDate: Date?

The date when the user last played the playlist entry’s item on this device.

var libraryAddedDate: Date?

The date when the user added the playlist entry’s item to the library.

var playCount: Int?

The number of times the user played the playlist entry’s item.

var playParameters: PlayParameters?

The parameters to use to play the playlist entry’s item.

var previewAssets: [PreviewAsset]?

The preview assets for the playlist entry’s item.

var releaseDate: Date?

The release date of the playlist entry’s item.

var title: String

The title of the playlist entry’s item.

var url: URL?

The URL for the playlist entry’s item.

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

MusicItem Implementations

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
- MusicPropertyContainer
- PlayableMusicItem
- Sendable

