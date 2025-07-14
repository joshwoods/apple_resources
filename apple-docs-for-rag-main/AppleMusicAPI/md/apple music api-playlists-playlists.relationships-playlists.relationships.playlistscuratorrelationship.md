

- Apple Music API
- Playlists
- Playlists.Relationships
-  Playlists.Relationships.PlaylistsCuratorRelationship 

Object

# Playlists.Relationships.PlaylistsCuratorRelationship

A relationship from the playlist to its curator.

Apple Music 1.0+

``` source
object Playlists.Relationships.PlaylistsCuratorRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[*]`

 (Required) 

The curator for the playlist.

Possible types: Activities`, `AppleCurators`, `Curators

## See Also

### Related Objects

object Playlists.Relationships.PlaylistsTracksRelationship

A relationship from the playlist to its tracks.

object Playlists.Relationships.PlaylistsLibraryRelationship

A relationship from the playlist to its library.

