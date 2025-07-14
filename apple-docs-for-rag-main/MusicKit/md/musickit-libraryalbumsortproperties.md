

- MusicKit
-  LibraryAlbumSortProperties 

Protocol

# LibraryAlbumSortProperties

Album properties your app uses to sort results for a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol LibraryAlbumSortProperties
```

## Topics

### Instance Properties

var artistName: String

The artist’s name.

**Required**

var lastPlayedDate: Date?

The date when the user last played the album on this device.

**Required**

var libraryAddedDate: Date?

The date when the user added the album to the library.

**Required**

var releaseDate: Date?

The release date (or expected prerelease date) for the album.

**Required**

var title: String

The title of the album.

**Required**

var trackCount: Int

The number of tracks for the album.

**Required**

