

- Apple Music API
- Albums
- Albums.Views
-  Albums.Views.AlbumsAppearsOnView 

Object

# Albums.Views.AlbumsAppearsOnView

A relationship view from this album to a selection of playlists tracks from this album appear on.

Apple Music 1.0+

``` source
object Albums.Views.AlbumsAppearsOnView
```

## Properties

`href`

`string`

The relative location to fetch the view directly.

`next`

`string`

The relative location to request the next page of resources in the collection, if additional resources are available for fetching.

`attributes`

Albums.Views.AlbumsAppearsOnView.Attributes

 (Required) 

The attributes for the view.

`data`

`[`Playlists`]`

 (Required) 

A selection of playlists that tracks from this album appear on.

## Topics

### Related Objects

object Albums.Views.AlbumsAppearsOnView.Attributes

The attributes for the view.

## See Also

### Related Objects

object Albums.Views.AlbumsOtherVersionsView

A relationship view for other versions of this album.

object Albums.Views.AlbumsRelatedAlbumsView

A relationship view from this album to related and similar albums.

object Albums.Views.AlbumsRelatedVideosView

A relationship view from this album to music videos for the songs on the album.

