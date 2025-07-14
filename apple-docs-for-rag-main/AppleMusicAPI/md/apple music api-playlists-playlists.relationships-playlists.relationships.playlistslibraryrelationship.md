

- Apple Music API
- Playlists
- Playlists.Relationships
-  Playlists.Relationships.PlaylistsLibraryRelationship 

Object

# Playlists.Relationships.PlaylistsLibraryRelationship

A relationship from the playlist to its library.

Apple Music 1.0+

``` source
object Playlists.Relationships.PlaylistsLibraryRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`LibraryPlaylists`]`

 (Required) 

The library for the playlist.

## See Also

### Related Objects

object Playlists.Relationships.PlaylistsCuratorRelationship

A relationship from the playlist to its curator.

object Playlists.Relationships.PlaylistsTracksRelationship

A relationship from the playlist to its tracks.

