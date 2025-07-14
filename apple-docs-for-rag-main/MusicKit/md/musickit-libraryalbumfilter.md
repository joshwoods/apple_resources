

- MusicKit
-  LibraryAlbumFilter 

Protocol

# LibraryAlbumFilter

Album properties your app uses as a filter for a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol LibraryAlbumFilter
```

## Topics

### Instance Properties

var artistName: String

The artist’s name.

**Required**

var artists: MusicItemCollection&lt;Artist>?

The album’s associated artists.

**Required**

var genres: MusicItemCollection&lt;Genre>?

The genres for the album.

**Required**

var id: MusicItemID

The unique identifier for the album.

**Required**

var isCompilation: Bool?

A Boolean value that indicates whether the album is a compilation.

**Required**

var title: String

The title of the album.

**Required**

