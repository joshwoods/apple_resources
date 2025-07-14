

- MusicKit
-  Artist 

Structure

# Artist

A music item that represents an artist.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Artist
```

## Topics

### Operators

static func == (Artist, Artist) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var albums: MusicItemCollection&lt;Album>?

The artist’s associated albums.

var appearsOnAlbums: MusicItemCollection&lt;Album>?

A collection of albums from other artists that this artist appears on.

var artwork: Artwork?

The artist artwork.

var compilationAlbums: MusicItemCollection&lt;Album>?

A collection of compilation albums that include tracks by the artist.

var editorialNotes: EditorialNotes?

The notes about the artist that appear in the Music catalog.

var featuredAlbums: MusicItemCollection&lt;Album>?

A collection of featured albums of the artist.

var featuredPlaylists: MusicItemCollection&lt;Playlist>?

A collection of the artist’s associated playlists.

var fullAlbums: MusicItemCollection&lt;Album>?

A collection of the artist’s full-release albums.

var genreNames: [String]?

The names of this artist’s associated genres.

var genres: MusicItemCollection&lt;Genre>?

The artist’s associated genres.

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the artist.

var latestRelease: Album?

The artist’s most recent album.

var libraryAddedDate: Date?

The date when the user added the artist to the library.

var liveAlbums: MusicItemCollection&lt;Album>?

A collection of the artist’s live albums.

var musicVideos: MusicItemCollection&lt;MusicVideo>?

The artist’s associated music videos.

var name: String

The name of the artist.

var playlists: MusicItemCollection&lt;Playlist>?

The artist’s associated playlists.

var similarArtists: MusicItemCollection&lt;Artist>?

A collection of artists similar to this artist.

var singles: MusicItemCollection&lt;Album>?

A collection of the artist’s associated albums in the *singles* category.

var station: Station?

The artist’s associated station.

var topMusicVideos: MusicItemCollection&lt;MusicVideo>?

A collection of the artist’s top music videos.

var topSongs: MusicItemCollection&lt;Song>?

A collection of the artist’s top songs.

var url: URL?

The URL for the artist.

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
- MusicCatalogSearchable
- MusicItem
- MusicLibraryRequestable
- MusicLibrarySearchable
- MusicLibrarySectionRequestable
- MusicPropertyContainer
- Sendable

## See Also

### Music Items

struct Album

A music item that represents an album.

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

