

- MusicKit
-  LibraryMusicVideoFilter 

Protocol

# LibraryMusicVideoFilter

Music video properties your app uses as a filter for a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol LibraryMusicVideoFilter
```

## Topics

### Instance Properties

var albumTitle: String?

The title of the album the music video appears on.

**Required**

var albums: MusicItemCollection&lt;Album>?

The music video’s associated albums.

**Required**

var artistName: String?

The artist’s name.

**Required**

var artists: MusicItemCollection&lt;Artist>?

The music video’s associated artists.

**Required**

var genres: MusicItemCollection&lt;Genre>?

The music video’s associated genres.

**Required**

var id: MusicItemID

The unique identifier for the music video.

**Required**

var title: String

The title of the music video.

**Required**

