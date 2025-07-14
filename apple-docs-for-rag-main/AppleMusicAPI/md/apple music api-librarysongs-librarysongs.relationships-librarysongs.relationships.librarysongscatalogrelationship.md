

- Apple Music API
- LibrarySongs
- LibrarySongs.Relationships
-  LibrarySongs.Relationships.LibrarySongsCatalogRelationship 

Object

# LibrarySongs.Relationships.LibrarySongsCatalogRelationship

A relationship from the library song to its associated catalog content.

Apple Music 1.0+

``` source
object LibrarySongs.Relationships.LibrarySongsCatalogRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`Songs`]`

 (Required) 

The song from the Apple Music catalog associated with the library song, if any.

## See Also

### Related Objects

object LibrarySongs.Relationships.LibrarySongsAlbumsRelationship

A relationship from the library song to its albums.

object LibrarySongs.Relationships.LibrarySongsArtistsRelationship

A relationship from the library song to its artists.

