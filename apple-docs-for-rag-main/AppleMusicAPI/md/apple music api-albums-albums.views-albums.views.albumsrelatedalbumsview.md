

- Apple Music API
- Albums
- Albums.Views
-  Albums.Views.AlbumsRelatedAlbumsView 

Object

# Albums.Views.AlbumsRelatedAlbumsView

A relationship view from this album to related and similar albums.

Apple Music 1.0+

``` source
object Albums.Views.AlbumsRelatedAlbumsView
```

## Properties

`href`

`string`

The relative location to fetch the view directly.

`next`

`string`

The relative location to request the next page of resources in the collection, if additional resources are available for fetching.

`attributes`

Albums.Views.AlbumsRelatedAlbumsView.Attributes

 (Required) 

The attributes for the view.

`data`

`[`Albums`]`

 (Required) 

A collection of other albums related or similar to the album.

## Topics

### Related Objects

object Albums.Views.AlbumsRelatedAlbumsView.Attributes

The attributes for the view.

## See Also

### Related Objects

object Albums.Views.AlbumsAppearsOnView

A relationship view from this album to a selection of playlists tracks from this album appear on.

object Albums.Views.AlbumsOtherVersionsView

A relationship view for other versions of this album.

object Albums.Views.AlbumsRelatedVideosView

A relationship view from this album to music videos for the songs on the album.

