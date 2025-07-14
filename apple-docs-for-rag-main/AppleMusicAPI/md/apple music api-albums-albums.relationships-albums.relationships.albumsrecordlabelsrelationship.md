

- Apple Music API
- Albums
- Albums.Relationships
-  Albums.Relationships.AlbumsRecordLabelsRelationship 

Object

# Albums.Relationships.AlbumsRecordLabelsRelationship

A relationship from the album to its associated record label.

Apple Music 1.0+

``` source
object Albums.Relationships.AlbumsRecordLabelsRelationship
```

## Properties

`href`

`string`

The relative location to fetch the relationship directly.

`next`

`string`

The relative location to request the next page of resources in the collection, if additional resources are available for fetching.

`data`

`[`RecordLabels`]`

 (Required) 

The album’s associated record label.

## See Also

### Related Objects

object Albums.Relationships.AlbumsArtistsRelationship

A relationship from the album to its artists.

object Albums.Relationships.AlbumsGenresRelationship

A relationship from the album to its genres.

object Albums.Relationships.AlbumsTracksRelationship

A relationship from the album to its tracks.

object Albums.Relationships.AlbumsLibraryRelationship

A relationship from the album to an associated library album.

