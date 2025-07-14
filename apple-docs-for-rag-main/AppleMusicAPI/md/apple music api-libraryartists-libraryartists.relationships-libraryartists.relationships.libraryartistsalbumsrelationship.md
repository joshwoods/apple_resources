

- Apple Music API
- LibraryArtists
- LibraryArtists.Relationships
-  LibraryArtists.Relationships.LibraryArtistsAlbumsRelationship 

Object

# LibraryArtists.Relationships.LibraryArtistsAlbumsRelationship

A relationship from the library artist to thier albums.

Apple Music 1.0+

``` source
object LibraryArtists.Relationships.LibraryArtistsAlbumsRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`LibraryAlbums`]`

 (Required) 

The albums for the library artist present in the user’s library.

## See Also

### Related Objects

object LibraryArtists.Relationships.LibraryArtistsCatalogRelationship

A relationship from the library artist to their associated catalog content.

