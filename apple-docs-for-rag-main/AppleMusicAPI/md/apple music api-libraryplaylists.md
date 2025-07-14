

- Apple Music API
-  LibraryPlaylists 

Object

# LibraryPlaylists

A resource object that represents a library playlist.

Apple Music 1.0+

``` source
object LibraryPlaylists
```

## Properties

`id`

`string`

 (Required) 

The identifier for the library playlist.

`type`

`string`

 (Required) 

This value is always `library-playlists`.

Value: `library-playlists`

`href`

`string`

 (Required) 

The relative location for the library playlist resource.

`attributes`

LibraryPlaylists.Attributes

The attributes for the library playlist.

`relationships`

LibraryPlaylists.Relationships

The relationships for the library playlist.

## Topics

### Related Objects

object LibraryPlaylists.Attributes

The attributes for a library playlist resource.

object LibraryPlaylists.Relationships

The relationships for a library playlist resource.

## See Also

### Handling the Response

object Playlists

A resource object that represents a playlist.

object PlaylistsResponse

The response to a playlists request.

object LibraryPlaylistsResponse

The response to a library playlists request.

object LibraryPlaylistsTracksRelationshipResponse

The response to a library playlists tracks relationship request.

object LibraryPlaylistFolders

A resource object that represents a library playlist folder.

object LibraryPlaylistFoldersResponse

The response to a library playlist folders request.

