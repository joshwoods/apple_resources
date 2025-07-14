

- Apple Music API
- LibrarySongs
-  LibrarySongs.Attributes 

Object

# LibrarySongs.Attributes

The attributes for a library song resource.

Apple Music 1.0+

``` source
object LibrarySongs.Attributes
```

## Properties

`albumName`

`string`

The name of the album the song appears on.

`artistName`

`string`

 (Required) 

The artist’s name.

`artwork`

Artwork

 (Required) 

The album artwork.

`contentRating`

`string`

The Recording Industry Association of America (RIAA) rating of the content. The possible values for this rating are `clean` and `explicit`. No value means no rating.

Possible Values: `clean, explicit`

`discNumber`

`integer`

The disc number the song appears on.

`durationInMillis`

`integer`

 (Required) 

The approximate length of the song in milliseconds.

`genreNames`

`[string]`

 (Required) 

The genre names the song is associated with.

`hasLyrics`

`boolean`

 (Required) 

Indicates if the song has lyrics available in the Apple Music catalog. If `true`, the song has lyrics available; otherwise, it does not.

`name`

`string`

 (Required) 

The localized name of the song.

`playParams`

PlayParameters

When present, this attribute indicates that the song is available to play. The value map may be used to initiate playback.

`releaseDate`

`string`

The release date of the song, when known, in YYYY-MM-DD or YYYY format. Pre-release songs may have an expected release date in the future.

`trackNumber`

`integer`

The number of the song in the album’s track list.

## See Also

### Related Objects

object LibrarySongs.Relationships

The relationships for a library song resource.

