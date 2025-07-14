

- Apple Music API
- Albums
- Albums.Relationships
-  Albums.Relationships.AlbumsArtistsRelationship 

Object

# Albums.Relationships.AlbumsArtistsRelationship

A relationship from the album to its artists.

Apple Music 1.0+

``` source
object Albums.Relationships.AlbumsArtistsRelationship
```

## Properties

`href`

`string`

The relative location to fetch the relationship directly.

`next`

`string`

The relative location to request the next page of resources in the collection, if additional resources are available for fetching.

`data`

`[`Artists`]`

 (Required) 

The artists for the album.

## See Also

### Related Objects

object Albums.Relationships.AlbumsGenresRelationship

A relationship from the album to its genres.

object Albums.Relationships.AlbumsTracksRelationship

A relationship from the album to its tracks.

object Albums.Relationships.AlbumsLibraryRelationship

A relationship from the album to an associated library album.

object Albums.Relationships.AlbumsRecordLabelsRelationship

A relationship from the album to its associated record label.

