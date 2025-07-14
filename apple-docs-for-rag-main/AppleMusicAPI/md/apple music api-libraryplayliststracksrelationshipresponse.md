

- Apple Music API
-  LibraryPlaylistsTracksRelationshipResponse 

Object

# LibraryPlaylistsTracksRelationshipResponse

The response to a library playlists tracks relationship request.

Apple Music 1.0+

``` source
object LibraryPlaylistsTracksRelationshipResponse
```

## Properties

`data`

`[*]`

 (Required) 

The Songs or doc:music-videos included in the response for the request.

Possible types: LibraryMusicVideos`, `LibrarySongs

`meta`

LibraryPlaylistsTracksRelationshipResponse.Meta

Meta data for this object.

`next`

`string`

The relative location to request the next page of resources in the collection, if additional resources are available for fetching.

## Topics

### Related Objects

object LibraryPlaylistsTracksRelationshipResponse.Meta

An object that represents the meta information for response to a library playlists tracks relationship request.

## See Also

### Handling the Response

object Playlists

A resource object that represents a playlist.

object PlaylistsResponse

The response to a playlists request.

object LibraryPlaylists

A resource object that represents a library playlist.

object LibraryPlaylistsResponse

The response to a library playlists request.

object LibraryPlaylistFolders

A resource object that represents a library playlist folder.

object LibraryPlaylistFoldersResponse

The response to a library playlist folders request.

