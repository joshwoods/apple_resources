

- Apple Music API
- MusicVideos
-  MusicVideos.Relationships 

Object

# MusicVideos.Relationships

The relationships for a music video resource.

Apple Music 1.0+

``` source
object MusicVideos.Relationships
```

## Properties

`albums`

MusicVideos.Relationships.MusicVideosAlbumsRelationship

The albums associated with the music video. By default, `albums` includes identifiers only.

Fetch limits: 10 default, 10 maximum.

`artists`

MusicVideos.Relationships.MusicVideosArtistsRelationship

The artists associated with the music video. By default, `artists` includes identifiers only.

Fetch limits: 10 default, 10 maximum.

`genres`

MusicVideos.Relationships.MusicVideosGenresRelationship

The genres associated with the music video. By default, `genres` not included.

Fetch limits: None.

`library`

MusicVideos.Relationships.MusicVideosLibraryRelationship

The library of a music video if added to library.

Fetch limits: None.

`songs`

MusicVideos.Relationships.MusicVideosSongsRelationship

The songs associated with the music video.

Fetch limits: 10 default, 10 maximum.

## Topics

### Related Objects

object MusicVideos.Relationships.MusicVideosAlbumsRelationship

A relationship from the music video to its albums.

object MusicVideos.Relationships.MusicVideosArtistsRelationship

A relationship from the music video to its artists.

object MusicVideos.Relationships.MusicVideosGenresRelationship

A relationship from the music video to its genres.

object MusicVideos.Relationships.MusicVideosLibraryRelationship

A relationship from the music video to its library.

object MusicVideos.Relationships.MusicVideosSongsRelationship

A relationship from the music video to its songs.

## See Also

### Related Objects

object MusicVideos.Attributes

The attributes for a music video resource.

object MusicVideos.Views

The views for a music video resource.

