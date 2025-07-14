

- Apple Music API
- Playlists
- Playlists.Relationships
-  Playlists.Relationships.PlaylistsTracksRelationship 

Object

# Playlists.Relationships.PlaylistsTracksRelationship

A relationship from the playlist to its tracks.

Apple Music 1.0+

``` source
object Playlists.Relationships.PlaylistsTracksRelationship
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

The ordered songs and music videos in the tracklist of the playlist.

Possible types: MusicVideos`, `Songs

## See Also

### Related Objects

object Playlists.Relationships.PlaylistsCuratorRelationship

A relationship from the playlist to its curator.

object Playlists.Relationships.PlaylistsLibraryRelationship

A relationship from the playlist to its library.

