

- Apple Music API
- LibraryPlaylists
- LibraryPlaylists.Relationships
-  LibraryPlaylists.Relationships.LibraryPlaylistsTracksRelationship 

Object

# LibraryPlaylists.Relationships.LibraryPlaylistsTracksRelationship

A relationship from the playlist to its tracks.

Apple Music 1.0+

``` source
object LibraryPlaylists.Relationships.LibraryPlaylistsTracksRelationship
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

The ordered library songs and library music videos in the tracklist of the playlist.

Possible types: LibraryMusicVideos`, `LibrarySongs

## See Also

### Related Objects

object LibraryPlaylists.Relationships.LibraryPlaylistsCatalogRelationship

A relationship from the playlist to its associated catalog content.

