

- Apple Music API
-  LibraryPlaylistFolders 

Object

# LibraryPlaylistFolders

A resource object that represents a library playlist folder.

Apple Music 1.0+

``` source
object LibraryPlaylistFolders
```

## Properties

`id`

`string`

 (Required) 

The identifier for the library playlist folder.

`type`

`string`

 (Required) 

This value is always `library-playlist-folders`.

Value: `library-playlist-folders`

`href`

`string`

 (Required) 

The relative location for the library playlist folder resource.

`attributes`

LibraryPlaylistFolders.Attributes

The attributes for the library-playlist-folders resource type.

`relationships`

LibraryPlaylistFolders.Relationships

The relationships from library-playlist-folders to other resources.

## Topics

### Related Objects

object LibraryPlaylistFolders.Attributes

A resource object that represents the attributes for a library playlist folder.

object LibraryPlaylistFolders.Relationships

A resource Object that represents the relationships for a library playlist folder.

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

object LibraryPlaylistsTracksRelationshipResponse

The response to a library playlists tracks relationship request.

object LibraryPlaylistFoldersResponse

The response to a library playlist folders request.

