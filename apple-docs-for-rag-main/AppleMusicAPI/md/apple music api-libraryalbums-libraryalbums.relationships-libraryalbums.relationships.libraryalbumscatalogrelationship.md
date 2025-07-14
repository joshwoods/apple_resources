

- Apple Music API
- LibraryAlbums
- LibraryAlbums.Relationships
-  LibraryAlbums.Relationships.LibraryAlbumsCatalogRelationship 

Object

# LibraryAlbums.Relationships.LibraryAlbumsCatalogRelationship

A relationship from the library album to its associated catalog content.

Apple Music 1.0+

``` source
object LibraryAlbums.Relationships.LibraryAlbumsCatalogRelationship
```

## Properties

`href`

`string`

The relative location to fetch the relationship directly.

`next`

`string`

The relative location to request the next page of resources in the collection, if additional resources are available for fetching.

`data`

`[`Albums`]`

 (Required) 

The album from the Apple Music catalog associated with the library album, if any.

## See Also

### Related Objects

object LibraryAlbums.Relationships.LibraryAlbumsArtistsRelationship

A relationship from the library album to its artist.

object LibraryAlbums.Relationships.LibraryAlbumsTracksRelationship

A relationship from the library album to its tracks.

