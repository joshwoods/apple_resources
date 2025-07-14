

- Apple Music API
- LibraryMusicVideos
-  LibraryMusicVideos.Attributes 

Object

# LibraryMusicVideos.Attributes

The attributes for the library music videos resource type.

Apple Music 1.0+

``` source
object LibraryMusicVideos.Attributes
```

## Properties

`albumName`

`string`

The name of the album the music video appears on.

`artistName`

`string`

 (Required) 

The artist’s name.

`artwork`

Artwork

 (Required) 

The artwork for the music video’s associated album.

`contentRating`

`string`

The Recording Industry Association of America (RIAA) rating of the content. The possible values for this rating are `clean` and `explicit`. No value means no rating.

Possible Values: `clean, explicit`

`durationInMillis`

`integer`

 (Required) 

The duration of the music video in milliseconds.

`genreNames`

`[string]`

 (Required) 

The names of the genres associated with this music video.

`name`

`string`

 (Required) 

The localized name of the music video.

`playParams`

PlayParameters

When present, this attribute indicates that the music video is able to play. The value map may be used to initiate playback.

`releaseDate`

`string`

The release date of the music video, when known, in YYYY-MM-DD or YYYY format. Pre-release content may have an expected release date in the future.

`trackNumber`

`integer`

The number of the music video in the album’s track list.

## See Also

### Related Objects

object LibraryMusicVideos.Relationships

The relationships from library music videos to other resources.

