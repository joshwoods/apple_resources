

- iTunes Library
-  ITLibAlbum 

Class

# ITLibAlbum

This class provides information about an album in the iTunes library.

Mac Catalyst 14.0+macOS 10.13+

``` source
class ITLibAlbum
```

## Overview

A *media item* is a track that iTunes associates with an album. See ITLibMediaItem.

A *compilation* is an album with tracks from more than one source.

If an album is part of a *multiple-disc set*, discNumber is the index of the album in the set.

To retrieve an ITLibAlbum instance, use the album property of ITLibMediaItem.

## Topics

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

### Deprecated

var artist: ITLibArtist?

The artist iTunes associates with the album.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Albums and Playlists

class ITLibPlaylist

This class describes a playlist in the iTunes library.

