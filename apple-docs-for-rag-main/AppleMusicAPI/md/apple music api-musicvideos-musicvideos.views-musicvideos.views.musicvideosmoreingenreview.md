

- Apple Music API
- MusicVideos
- MusicVideos.Views
-  MusicVideos.Views.MusicVideosMoreInGenreView 

Object

# MusicVideos.Views.MusicVideosMoreInGenreView

A relationship view from this music video to more music videos in a specific music video genre.

Apple Music 1.0+

``` source
object MusicVideos.Views.MusicVideosMoreInGenreView
```

## Properties

`href`

`string`

A relative location for the view.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the view if more exist.

`attributes`

MusicVideos.Views.MusicVideosMoreInGenreView.Attributes

 (Required) 

The attributes for the view.

`data`

`[`MusicVideos`]`

 (Required) 

Music videos in the given music video genre.

## Topics

### Related Objects

object MusicVideos.Views.MusicVideosMoreInGenreView.Attributes

More music videos in a specific music video genre.

## See Also

### Related Objects

object MusicVideos.Views.MusicVideosMoreByArtistView

A relationship view from this music video to more music videos of various types by the artist.

