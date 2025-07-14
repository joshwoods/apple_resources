

- MusicKit
-  Track 

Enumeration

# Track

A music item that represents a track.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Track
```

## Topics

### Operators

static func == (Track, Track) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case musicVideo(MusicVideo)

A track that corresponds to a music video.

case song(Song)

A track that corresponds to a song.

### Instance Properties

var albumTitle: String?

The title of the album the track appears on.

var albums: MusicItemCollection&lt;Album>?

The track’s associated albums.

var artistName: String

The artist’s name.

var artistURL: URL?

The artist’s URL.

var artists: MusicItemCollection&lt;Artist>?

The track’s associated artists.

var artwork: Artwork?

The artwork for the track.

var contentRating: ContentRating?

The rating of the content.

var discNumber: Int?

The disc number of the track.

var duration: TimeInterval?

The duration of the track.

var editorialNotes: EditorialNotes?

The editorial notes for the track.

var genreNames: [String]

The names of the track’s associated genres.

var genres: MusicItemCollection&lt;Genre>?

The track’s associated genres.

var hashValue: Int

The hash value.

var id: MusicItemID

The unique identifier for the track.

var isrc: String?

The International Standard Recording Code (ISRC) for the track.

var lastPlayedDate: Date?

The date when the user last played the track on this device.

var libraryAddedDate: Date?

The date when the user added the track to the library.

var playCount: Int?

The number of times the user played the track.

var playParameters: PlayParameters?

The parameters to use to play the track.

var previewAssets: [PreviewAsset]?

The preview assets for the track.

var releaseDate: Date?

The release date (or expected for pre-release) of the track.

var title: String

The title of the track.

var trackNumber: Int?

The track’s number in the album’s track list.

var url: URL?

The URL for the track.

var workName: String?

For classical music only, the name of the associated work.

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
- MusicRecentlyPlayedRequestable
- PlayableMusicItem
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

struct RecordLabel

A music item that represents a record label.

struct Song

A music item that represents a song.

struct Station

A music item that represents a station.

