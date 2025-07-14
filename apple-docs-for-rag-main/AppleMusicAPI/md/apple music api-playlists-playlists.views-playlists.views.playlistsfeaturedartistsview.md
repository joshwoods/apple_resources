

- Apple Music API
- Playlists
- Playlists.Views
-  Playlists.Views.PlaylistsFeaturedArtistsView 

Object

# Playlists.Views.PlaylistsFeaturedArtistsView

Artists that are featured on this playlist.

Apple Music 1.0+

``` source
object Playlists.Views.PlaylistsFeaturedArtistsView
```

## Properties

`href`

`string`

A relative location for the view.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the view if more exist.

`attributes`

Playlists.Views.PlaylistsFeaturedArtistsView.Attributes

 (Required) 

The attribute metadata for the view.

`data`

`[`Artists`]`

 (Required) 

A paginated collection of resources in the view.

## Topics

### Related Objects

object Playlists.Views.PlaylistsFeaturedArtistsView.Attributes

Attribute metadata for the playlist featured artists view.

## See Also

### Related Objects

object Playlists.Views.PlaylistsMoreByCuratorView

Additional content by the same curator for this playlist.

