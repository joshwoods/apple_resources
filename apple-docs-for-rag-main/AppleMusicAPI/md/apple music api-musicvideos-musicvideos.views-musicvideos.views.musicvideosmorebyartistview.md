

- Apple Music API
- MusicVideos
- MusicVideos.Views
-  MusicVideos.Views.MusicVideosMoreByArtistView 

Object

# MusicVideos.Views.MusicVideosMoreByArtistView

A relationship view from this music video to more music videos of various types by the artist.

Apple Music 1.0+

``` source
object MusicVideos.Views.MusicVideosMoreByArtistView
```

## Properties

`href`

`string`

A relative location for the view.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the view if more exist.

`attributes`

MusicVideos.Views.MusicVideosMoreByArtistView.Attributes

 (Required) 

The attributes for the view.

`data`

`[`MusicVideos`]`

 (Required) 

Music videos of some type by the artist.

## Topics

### Related Objects

object MusicVideos.Views.MusicVideosMoreByArtistView.Attributes

More content of some other type by the artist.

## See Also

### Related Objects

object MusicVideos.Views.MusicVideosMoreInGenreView

A relationship view from this music video to more music videos in a specific music video genre.

