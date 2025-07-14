

- Apple Music API
- Artists
- Artists.Relationships
-  Artists.Relationships.ArtistsAlbumsRelationship 

Object

# Artists.Relationships.ArtistsAlbumsRelationship

A relationship from the artist to its albums.

Apple Music 1.0+

``` source
object Artists.Relationships.ArtistsAlbumsRelationship
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

The albums for the artist.

## See Also

### Related Objects

object Artists.Relationships.ArtistsGenresRelationship

A relationship from the artist to its genres.

object Artists.Relationships.ArtistsMusicVideosRelationship

A relationship from the artist to its music videos.

object Artists.Relationships.ArtistsPlaylistsRelationship

A relationship from the artist to its playlists.

object Artists.Relationships.ArtistsStationRelationship

A relationship from the artist to its station.

