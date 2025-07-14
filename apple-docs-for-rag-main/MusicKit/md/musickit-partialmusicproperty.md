

- MusicKit
-  PartialMusicProperty 

Class

# PartialMusicProperty

A partially type-erased identifier for a music item property from a concrete root type to any resulting value type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class PartialMusicProperty
```

## Topics

### Type Properties

static let albums: MusicRelationshipProperty&lt;Artist, Album>

An identifier for the relationship property that returns the associated albums for the artist.

static let albums: MusicRelationshipProperty&lt;Song, Album>

An identifier for the relationship property that returns the associated albums for the song.

static let albums: MusicRelationshipProperty&lt;MusicVideo, Album>

An identifier of the relationship property that returns the associated albums for the music video.

static let appearsOn: MusicRelationshipProperty&lt;Album, Playlist>

An identifier for the association property that returns a collection of playlists that include tracks from the album.

static let appearsOnAlbums: MusicRelationshipProperty&lt;Artist, Album>

An identifier for the association property that returns a collection of albums from other artists that this artist appears on.

static var artistURL: MusicExtendedAttributeProperty&lt;MusicVideo, URL>

An identifier for the extended attribute property that returns the artist’s URL.

static var artistURL: MusicExtendedAttributeProperty&lt;Song, URL>

An identifier for the extended attribute property that returns the artist’s URL.

static var artistURL: MusicExtendedAttributeProperty&lt;Album, URL>

An identifier for the extended attribute property that returns the artist’s URL.

static let artists: MusicRelationshipProperty&lt;Album, Artist>

An identifier for the relationship property that returns the associated artists for the album.

static let artists: MusicRelationshipProperty&lt;Song, Artist>

An identifier for the relationship property that returns the associated artists for the song.

static let artists: MusicRelationshipProperty&lt;MusicVideo, Artist>

An identifier of the relationship property that returns the associated artists for the music video.

static let audioVariants: MusicExtendedAttributeProperty&lt;Song, [AudioVariant]>

An identifier for the extended attribute property that returns the audio variants for the song.

static let audioVariants: MusicExtendedAttributeProperty&lt;Album, [AudioVariant]>

An identifier for the extended attribute property that returns the audio variants for the album.

static let compilationAlbums: MusicRelationshipProperty&lt;Artist, Album>

An identifier for the association property that returns a collection of compilation albums that include tracks by the artist.

static let composers: MusicRelationshipProperty&lt;Song, Artist>

An identifier for the relationship property that returns the song’s composers.

static let curator: MusicRelationshipProperty&lt;Playlist, Curator>

An identifier for the extended attribute property that returns the playlist’s associated curator.

static let entries: MusicRelationshipProperty&lt;Playlist, Playlist.Entry>

An identifier for the relationship property that returns the entries in the playlist.

static let featuredAlbums: MusicRelationshipProperty&lt;Artist, Album>

An identifier for the association property that returns a collection of featured albums for the artist.

static let featuredArtists: MusicRelationshipProperty&lt;Playlist, Artist>

An identifier for the association property that returns a collection of featured artists for this playlist.

static let featuredPlaylists: MusicRelationshipProperty&lt;Artist, Playlist>

An identifier for the association property that returns a collection of the artist’s playlists.

static let fullAlbums: MusicRelationshipProperty&lt;Artist, Album>

An identifier for the association property that returns a collection of the artist’s full-release albums.

static let genres: MusicRelationshipProperty&lt;MusicVideo, Genre>

An identifier of the relationship property that returns the associated genres for the music video.

static let genres: MusicRelationshipProperty&lt;Artist, Genre>

An identifier for the relationship property that returns the associated genres for the artist.

static let genres: MusicRelationshipProperty&lt;Song, Genre>

An identifier for the relationship property that returns the associated genres for the song.

static let genres: MusicRelationshipProperty&lt;Album, Genre>

An identifier for the relationship property that returns the genres for the album.

static let latestRelease: MusicRelationshipProperty&lt;Artist, Album>

An identifier for the association property that returns the artist’s most recent album.

static var latestReleases: MusicRelationshipProperty&lt;RecordLabel, Album>

An identifier for the association property that returns a collection of the most recent releases for the record label.

static let liveAlbums: MusicRelationshipProperty&lt;Artist, Album>

An identifier for the association property that returns a collection of the artist’s live albums.

static let moreByArtist: MusicRelationshipProperty&lt;MusicVideo, MusicVideo>

An identifier of the association property that returns a collection of additional music videos by the artist.

static let moreByCurator: MusicRelationshipProperty&lt;Playlist, Playlist>

An identifier for the association property that returns a collection of additional playlists by the same curator.

static let moreInGenre: MusicRelationshipProperty&lt;MusicVideo, MusicVideo>

A identifier of the association property that returns a collection of music videos in the same genre as this music video.

static let musicVideos: MusicRelationshipProperty&lt;Artist, MusicVideo>

An identifier for the relationship property that returns the associated music videos for the artist.

static let musicVideos: MusicRelationshipProperty&lt;Song, MusicVideo>

An identifier for the relationship property that returns the song’s associated music videos.

static let otherVersions: MusicRelationshipProperty&lt;Album, Album>

An identifier for the association property that returns a collection of other versions of the album.

static let playlists: MusicRelationshipProperty&lt;Artist, Playlist>

An identifier for the relationship property that returns the associated playlists for the artist.

static let playlists: MusicRelationshipProperty&lt;Curator, Playlist>

An identifier for the relationship property that returns the associated playlists for the curator.

static let playlists: MusicRelationshipProperty&lt;RadioShow, Playlist>

An identifier for the relationship property that returns the associated playlists for the radio show.

static let radioShow: MusicRelationshipProperty&lt;Playlist, RadioShow>

An identifier for the extended attribute property that returns the playlist’s associated radio show.

static let recordLabels: MusicRelationshipProperty&lt;Album, RecordLabel>

An identifier for the relationship property that returns the record labels for the album.

static let relatedAlbums: MusicRelationshipProperty&lt;Album, Album>

An identifier for the association property that returns a collection of related albums.

static let relatedVideos: MusicRelationshipProperty&lt;Album, MusicVideo>

An identifier for the association property that returns a collection of related music videos for the album.

static let similarArtists: MusicRelationshipProperty&lt;Artist, Artist>

An identifier for the association property that returns a collection of artists similar to this artist.

static let singles: MusicRelationshipProperty&lt;Artist, Album>

An identifier of the association property that returns a collection of the artist’s albums in the *singles* category.

static let songs: MusicRelationshipProperty&lt;MusicVideo, Song>

An identifier of the relationship property that returns the associated songs for the music video.

static let station: MusicRelationshipProperty&lt;Song, Station>

An identifier for the relationship property that returns the associated station for the song.

static let station: MusicRelationshipProperty&lt;Artist, Station>

An identifier for the relationship property that returns the associated station for the artist.

static let topMusicVideos: MusicRelationshipProperty&lt;Artist, MusicVideo>

An identifier for the association property that returns a collection of the artist’s top music videos.

static var topReleases: MusicRelationshipProperty&lt;RecordLabel, Album>

An identifier for the association property that returns a collection of top releases for the record label.

static let topSongs: MusicRelationshipProperty&lt;Artist, Song>

An identifier for the association property that returns a collection of the artist’s top songs.

static let tracks: MusicRelationshipProperty&lt;Playlist, Track>

An identifier for the relationship property that returns the tracks in the playlist.

static let tracks: MusicRelationshipProperty&lt;Album, Track>

An identifier for the relationship property that returns the tracks on the album.

## Relationships

### Inherits From

- AnyMusicProperty

### Inherited By

- MusicAttributeProperty
- PartialMusicAsyncProperty

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Utility

protocol MusicItem

A protocol with basic requirements for music items.

struct MusicItemID

An object that represents a unique identifier for a music item.

struct MusicItemCollection

A collection of music items.

protocol MusicPropertyContainer

A protocol for music items that allow loading additional properties that you can fetch asynchronously.

class MusicRelationshipProperty

An identifier for a music item relationship property from a specific root type to a specific value type for the element of the resulting collection.

class MusicExtendedAttributeProperty

An identifier for a music item extended attribute property from a specific root type to a specific resulting value type.

class MusicAttributeProperty

An identifier for a music item attribute property from a specific root type to a specific resulting value type.

class PartialMusicAsyncProperty

A partially type-erased identifier for a music item property that you can fetch asynchronously from a concrete root type to any resulting value type.

class AnyMusicProperty

A type-erased identifier for a music item property, from any root type to any resulting value type.

