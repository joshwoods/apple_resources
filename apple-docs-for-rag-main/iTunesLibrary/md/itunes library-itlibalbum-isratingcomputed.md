

- iTunes Library
- ITLibAlbum
-  isRatingComputed 

Instance Property

# isRatingComputed

A Boolean value that indicates whether the system computes the rating of the album using the ratings of individual tracks in the album.

Mac Catalyst 14.0+macOS 10.13+

``` source
var isRatingComputed: Bool { get }
```

## Discussion

If the user rates tracks within the album individually, but hasn’t assigned a specific rating for the album, the album rating computes as the average of the rating of all tracks within the album (tracks with no rating don’t affect this average), and this property is `true`.

If the user has rated the album, this property is `false`.

If the user hasn’t rated the album and hasn’t rated any tracks on this album, the property is `false`.

## See Also

### Getting Album Info

var trackCount: Int

The number of tracks in the album.

var title: String?

The title of the album.

var sortTitle: String?

The title to use when sorting by album title.

var rating: Int

The rating of the album.

var isGapless: Bool

A Boolean value that indicates whether the album is gapless.

var discNumber: Int

The index (1, 2, 3, and so on) of the disc within an album that’s a multiple-disc set.

var discCount: Int

The number of discs in a multiple-disc set.

var isCompilation: Bool

A Boolean value that indicates whether the album is a compilation.

var albumArtist: String?

The name of the artist iTunes associates with the album.

var sortAlbumArtist: String?

The name to use when sorting by album artist.

var persistentID: NSNumber

The unique identifier of the album.

