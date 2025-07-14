

- Apple Music API
- LibraryAlbums
- LibraryAlbums.Relationships
-  LibraryAlbums.Relationships.LibraryAlbumsTracksRelationship 

Object

# LibraryAlbums.Relationships.LibraryAlbumsTracksRelationship

A relationship from the library album to its tracks.

Apple Music 1.0+

``` source
object LibraryAlbums.Relationships.LibraryAlbumsTracksRelationship
```

## Properties

`href`

`string`

The relative location to fetch the relationship directly.

`next`

`string`

The relative location to request the next page of resources in the collection, if additional resources are available for fetching.

`data`

`[*]`

 (Required) 

The songs and music videos from the library album’s tracklist added to the user’s library.

Possible types: LibraryMusicVideos`, `LibrarySongs

## See Also

### Related Objects

object LibraryAlbums.Relationships.LibraryAlbumsArtistsRelationship

A relationship from the library album to its artist.

object LibraryAlbums.Relationships.LibraryAlbumsCatalogRelationship

A relationship from the library album to its associated catalog content.

