

- Apple Music API
- Albums
- Albums.Views
-  Albums.Views.AlbumsRelatedVideosView 

Object

# Albums.Views.AlbumsRelatedVideosView

A relationship view from this album to music videos for the songs on the album.

Apple Music 1.0+

``` source
object Albums.Views.AlbumsRelatedVideosView
```

## Properties

`href`

`string`

The relative location to fetch the view directly.

`next`

`string`

The relative location to request the next page of resources in the collection, if additional resources are available for fetching.

`attributes`

Albums.Views.AlbumsRelatedVideosView.Attributes

 (Required) 

The attributes for the view.

`data`

`[`MusicVideos`]`

 (Required) 

The music videos available for songs on the album.

## Topics

### Related Objects

object Albums.Views.AlbumsRelatedVideosView.Attributes

The attributes for the view.

## See Also

### Related Objects

object Albums.Views.AlbumsAppearsOnView

A relationship view from this album to a selection of playlists tracks from this album appear on.

object Albums.Views.AlbumsOtherVersionsView

A relationship view for other versions of this album.

object Albums.Views.AlbumsRelatedAlbumsView

A relationship view from this album to related and similar albums.

