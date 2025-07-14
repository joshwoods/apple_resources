

- Apple Music API
- MusicVideos
- MusicVideos.Relationships
-  MusicVideos.Relationships.MusicVideosAlbumsRelationship 

Object

# MusicVideos.Relationships.MusicVideosAlbumsRelationship

A relationship from the music video to its albums.

Apple Music 1.0+

``` source
object MusicVideos.Relationships.MusicVideosAlbumsRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`Albums`]`

 (Required) 

The albums associated with the music video, if any.

## See Also

### Related Objects

object MusicVideos.Relationships.MusicVideosArtistsRelationship

A relationship from the music video to its artists.

object MusicVideos.Relationships.MusicVideosGenresRelationship

A relationship from the music video to its genres.

object MusicVideos.Relationships.MusicVideosLibraryRelationship

A relationship from the music video to its library.

object MusicVideos.Relationships.MusicVideosSongsRelationship

A relationship from the music video to its songs.

