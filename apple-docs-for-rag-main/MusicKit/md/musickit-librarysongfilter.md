

- MusicKit
-  LibrarySongFilter 

Protocol

# LibrarySongFilter

Song properties your app uses as a filter for a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol LibrarySongFilter
```

## Topics

### Instance Properties

var albumTitle: String?

The title of the album the song appears on.

**Required**

var albums: MusicItemCollection&lt;Album>?

The song’s associated albums.

**Required**

var artistName: String?

The artist’s name.

**Required**

var artists: MusicItemCollection&lt;Artist>?

The song’s associated artists.

**Required**

var composerName: String?

The name of the song’s composer.

**Required**

var genres: MusicItemCollection&lt;Genre>?

The song’s associated genres.

**Required**

var id: MusicItemID

The unique identifier for the song.

**Required**

var title: String

The title of the song.

**Required**

