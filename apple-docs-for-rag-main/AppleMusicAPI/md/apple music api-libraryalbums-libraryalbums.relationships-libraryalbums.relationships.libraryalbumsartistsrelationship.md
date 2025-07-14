

- Apple Music API
- LibraryAlbums
- LibraryAlbums.Relationships
-  LibraryAlbums.Relationships.LibraryAlbumsArtistsRelationship 

Object

# LibraryAlbums.Relationships.LibraryAlbumsArtistsRelationship

A relationship from the library album to its artist.

Apple Music 1.0+

``` source
object LibraryAlbums.Relationships.LibraryAlbumsArtistsRelationship
```

## Properties

`href`

`string`

The relative location to fetch the relationship directly.

`next`

`string`

The relative location to request the next page of resources in the collection, if additional resources are available for fetching.

`data`

`[`LibraryArtists`]`

 (Required) 

The library artists for the library album.

## See Also

### Related Objects

object LibraryAlbums.Relationships.LibraryAlbumsCatalogRelationship

A relationship from the library album to its associated catalog content.

object LibraryAlbums.Relationships.LibraryAlbumsTracksRelationship

A relationship from the library album to its tracks.

