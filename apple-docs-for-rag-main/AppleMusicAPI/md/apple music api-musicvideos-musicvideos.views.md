

- Apple Music API
- MusicVideos
-  MusicVideos.Views 

Object

# MusicVideos.Views

The views for a music video resource.

Apple Music 1.0+

``` source
object MusicVideos.Views
```

## Properties

`more-by-artist`

MusicVideos.Views.MusicVideosMoreByArtistView

More music videos of some type by the artist.

Fetch limits: 15 default, 100 maximum.

`more-in-genre`

MusicVideos.Views.MusicVideosMoreInGenreView

More music videos in the given music video genre.

Fetch limits: 15 default, 100 maximum.

## Topics

### Related Objects

object MusicVideos.Views.MusicVideosMoreByArtistView

A relationship view from this music video to more music videos of various types by the artist.

object MusicVideos.Views.MusicVideosMoreInGenreView

A relationship view from this music video to more music videos in a specific music video genre.

## See Also

### Related Objects

object MusicVideos.Attributes

The attributes for a music video resource.

object MusicVideos.Relationships

The relationships for a music video resource.

