

- Apple Music API
- Songs
- Songs.Relationships
-  Songs.Relationships.SongsLibraryRelationship 

Object

# Songs.Relationships.SongsLibraryRelationship

A relationship from the song to its library.

Apple Music 1.0+

``` source
object Songs.Relationships.SongsLibraryRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`LibrarySongs`]`

 (Required) 

The library associated with the song.

## See Also

### Related Objects

object Songs.Relationships.SongsAlbumsRelationship

A relationship from the song to its albums.

object Songs.Relationships.SongsArtistsRelationship

A relationship from the song to its artists.

object Songs.Relationships.SongsGenresRelationship

A relationship from the song to its genres.

object Songs.Relationships.SongsComposersRelationship

A relationship from the song to its composers.

object Songs.Relationships.SongsMusicVideosRelationship

A relationship from the song to its music videos.

object Songs.Relationships.SongsStationRelationship

A relationship from the song to its station.

