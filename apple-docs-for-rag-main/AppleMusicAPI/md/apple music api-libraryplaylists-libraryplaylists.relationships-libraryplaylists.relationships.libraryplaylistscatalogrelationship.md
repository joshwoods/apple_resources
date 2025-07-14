

- Apple Music API
- LibraryPlaylists
- LibraryPlaylists.Relationships
-  LibraryPlaylists.Relationships.LibraryPlaylistsCatalogRelationship 

Object

# LibraryPlaylists.Relationships.LibraryPlaylistsCatalogRelationship

A relationship from the playlist to its associated catalog content.

Apple Music 1.0+

``` source
object LibraryPlaylists.Relationships.LibraryPlaylistsCatalogRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`Playlists`]`

 (Required) 

The playlist from the Apple Music catalog associated with the library playlist, if any.

## See Also

### Related Objects

object LibraryPlaylists.Relationships.LibraryPlaylistsTracksRelationship

A relationship from the playlist to its tracks.

