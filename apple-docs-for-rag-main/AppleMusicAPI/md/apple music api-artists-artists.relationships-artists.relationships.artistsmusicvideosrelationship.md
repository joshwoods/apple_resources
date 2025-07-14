

- Apple Music API
- Artists
- Artists.Relationships
-  Artists.Relationships.ArtistsMusicVideosRelationship 

Object

# Artists.Relationships.ArtistsMusicVideosRelationship

A relationship from the artist to its music videos.

Apple Music 1.0+

``` source
object Artists.Relationships.ArtistsMusicVideosRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`MusicVideos`]`

 (Required) 

The music videos for the artist.

## See Also

### Related Objects

object Artists.Relationships.ArtistsAlbumsRelationship

A relationship from the artist to its albums.

object Artists.Relationships.ArtistsGenresRelationship

A relationship from the artist to its genres.

object Artists.Relationships.ArtistsPlaylistsRelationship

A relationship from the artist to its playlists.

object Artists.Relationships.ArtistsStationRelationship

A relationship from the artist to its station.

