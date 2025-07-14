

- Apple Music API
- LibrarySongs
- LibrarySongs.Relationships
-  LibrarySongs.Relationships.LibrarySongsAlbumsRelationship 

Object

# LibrarySongs.Relationships.LibrarySongsAlbumsRelationship

A relationship from the library song to its albums.

Apple Music 1.0+

``` source
object LibrarySongs.Relationships.LibrarySongsAlbumsRelationship
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

The albums in the library associated with the song.

## See Also

### Related Objects

object LibrarySongs.Relationships.LibrarySongsArtistsRelationship

A relationship from the library song to its artists.

object LibrarySongs.Relationships.LibrarySongsCatalogRelationship

A relationship from the library song to its associated catalog content.

