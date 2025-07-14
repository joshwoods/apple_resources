

- Apple Music API
- Playlists
- Playlists.Views
-  Playlists.Views.PlaylistsMoreByCuratorView 

Object

# Playlists.Views.PlaylistsMoreByCuratorView

Additional content by the same curator for this playlist.

Apple Music 1.0+

``` source
object Playlists.Views.PlaylistsMoreByCuratorView
```

## Properties

`href`

`string`

A relative location for the view.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the view if more exist.

`attributes`

Playlists.Views.PlaylistsMoreByCuratorView.Attributes

 (Required) 

The attribute metadata for the view.

`data`

`[`Playlists`]`

 (Required) 

A paginated collection of resources in the view.

## Topics

### Related Objects

object Playlists.Views.PlaylistsMoreByCuratorView.Attributes

Attribute metadata for the view containing additional content by the same curator for this playlist.

## See Also

### Related Objects

object Playlists.Views.PlaylistsFeaturedArtistsView

Artists that are featured on this playlist.

