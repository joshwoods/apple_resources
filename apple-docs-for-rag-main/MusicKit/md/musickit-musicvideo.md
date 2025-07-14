

- MusicKit
-  MusicVideo 

Structure

# MusicVideo

A music item that represents a music video.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MusicVideo
```

## Topics

### Operators

static func == (MusicVideo, MusicVideo) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var albumTitle: String?

The title of the album the music video appears on.

var albums: MusicItemCollection&lt;Album>?

The music video’s associated albums.

var artistName: String

The artist’s name.

var artistURL: URL?

The artist’s URL.

var artists: MusicItemCollection&lt;Artist>?

The music video’s associated artists.

var artwork: Artwork?

The artwork for the music video.

var contentRating: ContentRating?

The rating of the content.

var duration: TimeInterval?

The duration of the music video.

var editorialNotes: EditorialNotes?

The editorial notes for the music video.

var genreNames: [String]

The names of the music video’s associated genres.

var genres: MusicItemCollection&lt;Genre>?

The music video’s associated genres.

var has4K: Bool?

A Boolean value that indicates whether the music video has 4K content.

var hasHDR: Bool?

A Boolean value that indicates whether the music video has HDR10-encoded content.

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the music video.

var isPreview: Bool

A Boolean value that indicates whether this content corresponds to a subscription video preview.

var isrc: String?

The International Standard Recording Code (ISRC) for the music video.

var lastPlayedDate: Date?

The date when the user last played the music video on this device.

var libraryAddedDate: Date?

The date when the user added the music video to the library.

var moreByArtist: MusicItemCollection&lt;MusicVideo>?

A collection of additional music videos by the artist.

var moreInGenre: MusicItemCollection&lt;MusicVideo>?

A collection of music videos in the same genre as this music video.

var playCount: Int?

The number of times the user played the music video.

var playParameters: PlayParameters?

The parameters to use to play the music video.

var previewAssets: [PreviewAsset]?

The preview assets for the music video.

var releaseDate: Date?

The release date (or expected prerelease date) for the music video.

var songs: MusicItemCollection&lt;Song>?

The music video’s associated songs.

var title: String

The title of the music video.

var trackNumber: Int?

The music video’s number in the album’s track list.

var url: URL?

The URL for the music video.

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

