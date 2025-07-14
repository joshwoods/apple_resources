

- Apple Music API
- MusicVideos
- MusicVideos.Relationships
-  MusicVideos.Relationships.MusicVideosGenresRelationship 

Object

# MusicVideos.Relationships.MusicVideosGenresRelationship

A relationship from the music video to its genres.

Apple Music 1.0+

``` source
object MusicVideos.Relationships.MusicVideosGenresRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`Genres`]`

 (Required) 

The genres associated with the music video.

## See Also

### Related Objects

object MusicVideos.Relationships.MusicVideosAlbumsRelationship

A relationship from the music video to its albums.

object MusicVideos.Relationships.MusicVideosArtistsRelationship

A relationship from the music video to its artists.

object MusicVideos.Relationships.MusicVideosLibraryRelationship

A relationship from the music video to its library.

object MusicVideos.Relationships.MusicVideosSongsRelationship

A relationship from the music video to its songs.

