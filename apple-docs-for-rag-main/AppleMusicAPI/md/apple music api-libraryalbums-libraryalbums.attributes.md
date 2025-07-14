

- Apple Music API
- LibraryAlbums
-  LibraryAlbums.Attributes 

Object

# LibraryAlbums.Attributes

The attributes for a library album resource.

Apple Music 1.0+

``` source
object LibraryAlbums.Attributes
```

## Properties

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

`dateAdded`

`string`

The date the album was added to the library, in YYYY-MM-DD or YYYY format.

`name`

`string`

 (Required) 

The localized name of the album.

`playParams`

PlayParameters

When present, this attribute indicates that tracks from the album are available to play. The value map may be used to initiate playback of available tracks on the album.

`releaseDate`

`string`

The release date of the album, when known, in YYYY-MM-DD or YYYY format. Pre-release albums may have an expected release date in the future.

`trackCount`

`integer`

 (Required) 

The number of tracks.

`genreNames`

`[string]`

 (Required) 

The names of the genres associated with this album.

## See Also

### Related Objects

object LibraryAlbums.Relationships

The relationships for a library album object.

