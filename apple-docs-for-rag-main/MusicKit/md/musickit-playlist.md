

- MusicKit
-  Playlist 

Structure

# Playlist

A music item that represents a playlist.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Playlist
```

## Topics

### Structures

struct Entry

A music item that represents a playlist entry.

### Operators

static func == (Playlist, Playlist) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var artwork: Artwork?

The artwork for the playlist.

var curator: Curator?

The playlist’s associated curator.

var curatorName: String?

The display name for the playlist’s curator.

var entries: MusicItemCollection&lt;Playlist.Entry>?

The entries in the playlist

var featuredArtists: MusicItemCollection&lt;Artist>?

A collection of featured artists for this playlist.

var hashValue: Int

The hash value.

let id: MusicItemID

The unique identifier for the playlist.

var isChart: Bool?

A Boolean value that indicates whether the playlist represents a popularity chart.

var kind: Playlist.Kind?

The kind of playlist.

var lastModifiedDate: Date?

The playlist’s most recent modification date.

var lastPlayedDate: Date?

The date when the user last played the playlist on this device.

var libraryAddedDate: Date?

The date when the user added the playlist to the library.

var moreByCurator: MusicItemCollection&lt;Playlist>?

A collection of additional playlists by the same curator.

var name: String

The name of the playlist.

var playParameters: PlayParameters?

The parameters to use to play the tracks in the playlist.

var radioShow: RadioShow?

The playlist’s associated radio show.

var shortDescription: String?

An abbreviated description to show inline or when the playlist appears alongside other content.

var standardDescription: String?

A description to show when the playlist is prominently displayed.

var tracks: MusicItemCollection&lt;Track>?

The tracks in the playlist.

var url: URL?

The URL for the playlist.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Enumerations

enum Kind

The available kinds of playlists.

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

