

- MusicKit
-  LibraryArtistFilter 

Protocol

# LibraryArtistFilter

Artist properties your app uses as a filter for a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol LibraryArtistFilter
```

## Topics

### Instance Properties

var genres: MusicItemCollection&lt;Genre>?

The artist’s associated genres.

**Required**

var id: MusicItemID

The unique identifier for the artist.

**Required**

var name: String

The name of the artist.

**Required**

var playlists: MusicItemCollection&lt;Playlist>?

The artist’s associated playlists.

**Required**

