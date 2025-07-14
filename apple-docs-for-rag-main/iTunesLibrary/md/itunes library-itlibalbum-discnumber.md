

- iTunes Library
- ITLibAlbum
-  discNumber 

Instance Property

# discNumber

The index (1, 2, 3, and so on) of the disc within an album that’s a multiple-disc set.

Mac Catalyst 14.0+macOS 10.13+

``` source
var discNumber: Int { get }
```

## Discussion

If the album isn’t part of a multiple-disc set, this property is `0`.

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

var isRatingComputed: Bool

A Boolean value that indicates whether the system computes the rating of the album using the ratings of individual tracks in the album.

var isGapless: Bool

A Boolean value that indicates whether the album is gapless.

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

