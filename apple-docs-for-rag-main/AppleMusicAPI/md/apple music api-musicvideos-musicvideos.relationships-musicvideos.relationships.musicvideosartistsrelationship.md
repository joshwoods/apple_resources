

- Apple Music API
- MusicVideos
- MusicVideos.Relationships
-  MusicVideos.Relationships.MusicVideosArtistsRelationship 

Object

# MusicVideos.Relationships.MusicVideosArtistsRelationship

A relationship from the music video to its artists.

Apple Music 1.0+

``` source
object MusicVideos.Relationships.MusicVideosArtistsRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`Artists`]`

 (Required) 

The artists associated with the music video.

## See Also

### Related Objects

object MusicVideos.Relationships.MusicVideosAlbumsRelationship

A relationship from the music video to its albums.

object MusicVideos.Relationships.MusicVideosGenresRelationship

A relationship from the music video to its genres.

object MusicVideos.Relationships.MusicVideosLibraryRelationship

A relationship from the music video to its library.

object MusicVideos.Relationships.MusicVideosSongsRelationship

A relationship from the music video to its songs.

