

- MusicKit
-  Album 

Structure

# Album

A music item that represents an album.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Album
```

## Topics

### Operators

static func == (Album, Album) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var appearsOn: MusicItemCollection&lt;Playlist>?

A collection of playlists that include tracks from the album.

var artistName: String

The artist’s name.

var artistURL: URL?

The artist’s URL.

var artists: MusicItemCollection&lt;Artist>?

The album’s associated artists.

var artwork: Artwork?

The album artwork.

var audioVariants: [AudioVariant]?

The variants that indicate the quality of audio available for the album.

var contentRating: ContentRating?

The rating of the content.

var copyright: String?

The copyright text for the album.

var editorialNotes: EditorialNotes?

The notes about the album that appear in the Music app.

var genreNames: [String]

The names of the album’s associated genres.

var genres: MusicItemCollection&lt;Genre>?

The genres for the album.

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the album.

var isAppleDigitalMaster: Bool?

A Boolean value that indicates whether the album is an Apple Digital Master.

var isCompilation: Bool?

A Boolean value that indicates whether the album is a compilation.

var isComplete: Bool?

A Boolean value that indicates whether the album is complete.

var isSingle: Bool?

A Boolean value that indicates whether the album consists of a single song.

var lastPlayedDate: Date?

The date when the user last played the album on this device.

var libraryAddedDate: Date?

The date when the user added the album to the library.

var otherVersions: MusicItemCollection&lt;Album>?

A collection of other versions of the album.

var playParameters: PlayParameters?

The parameters to use to play the tracks of the album.

var recordLabelName: String?

The name of the album’s record label.

var recordLabels: MusicItemCollection&lt;RecordLabel>?

The record labels for the album.

var relatedAlbums: MusicItemCollection&lt;Album>?

A collection of related albums.

var relatedVideos: MusicItemCollection&lt;MusicVideo>?

A collection of the album’s music videos.

var releaseDate: Date?

The release date (or expected prerelease date) for the album.

var title: String

The title of the album.

var trackCount: Int

The number of tracks for the album.

var tracks: MusicItemCollection&lt;Track>?

The tracks on the album.

var upc: String?

The universal product code (UPC) for the album.

var url: URL?

The URL for the album.

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
- MusicLibrarySectionRequestable
- MusicPersonalRecommendationItem
- MusicPlaylistAddable
- MusicPropertyContainer
- PlayableMusicItem
- Sendable

## See Also

### Music Items

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

enum Track

A music item that represents a track.

