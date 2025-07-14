

- MusicKit
-  Song 

Structure

# Song

A music item that represents a song.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Song
```

## Topics

### Operators

static func == (Song, Song) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var albumTitle: String?

The title of the album the song appears on.

var albums: MusicItemCollection&lt;Album>?

The song’s associated albums.

var artistName: String

The artist’s name.

var artistURL: URL?

The artist’s URL.

var artists: MusicItemCollection&lt;Artist>?

The song’s associated artists.

var artwork: Artwork?

The artwork for the song.

var attribution: String?

For classical music only, the name of the artist or composer to attribute to the song.

var audioVariants: [AudioVariant]?

The variants that indicate the quality of audio available for the song.

var composerName: String?

The name of the song’s composer.

var composers: MusicItemCollection&lt;Artist>?

The song’s composers.

var contentRating: ContentRating?

The rating of the content.

var discNumber: Int?

The number of the disc the song appears on.

var duration: TimeInterval?

The duration of the song.

var editorialNotes: EditorialNotes?

The editorial notes for the song.

var genreNames: [String]

The names of the song’s associated genres.

var genres: MusicItemCollection&lt;Genre>?

The song’s associated genres.

var hasLyrics: Bool

A Boolean value that indicates whether the song has lyrics available in the catalog. If true, the song has lyrics available; otherwise, it doesn’t.

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the song.

var isAppleDigitalMaster: Bool?

A Boolean value that indicates whether the song is an Apple Digital Master.

var isrc: String?

The International Standard Recording Code (ISRC) for the song.

var lastPlayedDate: Date?

The date when the user last played the song on this device.

var libraryAddedDate: Date?

The date when the user added the song to the library.

var movementCount: Int?

For classical music only, the movement count of this song.

var movementName: String?

For classical music only, the movement name of this song.

var movementNumber: Int?

For classical music only, the movement number of this song.

var musicVideos: MusicItemCollection&lt;MusicVideo>?

The song’s associated music videos.

var playCount: Int?

The number of times the user played the song.

var playParameters: PlayParameters?

The parameters to use to play the song.

var previewAssets: [PreviewAsset]?

The preview assets for the song.

var releaseDate: Date?

The release date (or expected prerelease date) for the song.

var station: Station?

The song’s associated station.

var title: String

The title of the song.

var trackNumber: Int?

The song’s number in the album’s track list.

var url: URL?

The URL for the song.

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
- MusicCatalogChartRequestable
- MusicCatalogSearchable
- MusicItem
- MusicLibraryAddable
- MusicLibraryRequestable
- MusicLibrarySearchable
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

struct Station

A music item that represents a station.

enum Track

A music item that represents a track.

