

- Apple Music API
- Albums
- Albums.Relationships
-  Albums.Relationships.AlbumsGenresRelationship 

Object

# Albums.Relationships.AlbumsGenresRelationship

A relationship from the album to its genres.

Apple Music 1.0+

``` source
object Albums.Relationships.AlbumsGenresRelationship
```

## Properties

`href`

`string`

The relative location to fetch the relationship directly.

`next`

`string`

The relative location to request the next page of resources in the collection, if additional resources are available for fetching.

`data`

`[`Genres`]`

 (Required) 

The album’s associated genre.

## See Also

### Related Objects

object Albums.Relationships.AlbumsArtistsRelationship

A relationship from the album to its artists.

object Albums.Relationships.AlbumsTracksRelationship

A relationship from the album to its tracks.

object Albums.Relationships.AlbumsLibraryRelationship

A relationship from the album to an associated library album.

object Albums.Relationships.AlbumsRecordLabelsRelationship

A relationship from the album to its associated record label.

