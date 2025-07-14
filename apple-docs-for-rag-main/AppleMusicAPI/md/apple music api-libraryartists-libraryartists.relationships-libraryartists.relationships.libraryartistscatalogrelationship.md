

- Apple Music API
- LibraryArtists
- LibraryArtists.Relationships
-  LibraryArtists.Relationships.LibraryArtistsCatalogRelationship 

Object

# LibraryArtists.Relationships.LibraryArtistsCatalogRelationship

A relationship from the library artist to their associated catalog content.

Apple Music 1.0+

``` source
object LibraryArtists.Relationships.LibraryArtistsCatalogRelationship
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

The artist from the Apple Music catalog associated with the library artist, if any.

## See Also

### Related Objects

object LibraryArtists.Relationships.LibraryArtistsAlbumsRelationship

A relationship from the library artist to thier albums.

