

- Apple Music API
-  Playlists 

Object

# Playlists

A resource object that represents a playlist.

Apple Music 1.0+

``` source
object Playlists
```

## Properties

`id`

`string`

 (Required) 

The identifier for the playlist.

`type`

`string`

 (Required) 

This value is always `playlists`.

Value: `playlists`

`href`

`string`

 (Required) 

The relative location for the playlist resource.

`attributes`

Playlists.Attributes

The attributes for the playlist.

`relationships`

Playlists.Relationships

The relationships for the playlist.

`views`

Playlists.Views

The views for associations between playlists and other resources.

## Topics

### Related Objects

object Playlists.Attributes

The attributes for a playlist resource.

object Playlists.Relationships

The relationships for a playlist resource.

object Playlists.Views

The views for a music video resource.

## See Also

### Handling the Response

object PlaylistsResponse

The response to a playlists request.

object LibraryPlaylists

A resource object that represents a library playlist.

object LibraryPlaylistsResponse

The response to a library playlists request.

object LibraryPlaylistsTracksRelationshipResponse

The response to a library playlists tracks relationship request.

object LibraryPlaylistFolders

A resource object that represents a library playlist folder.

object LibraryPlaylistFoldersResponse

The response to a library playlist folders request.

