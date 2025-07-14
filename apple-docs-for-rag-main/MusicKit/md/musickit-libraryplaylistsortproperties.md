

- MusicKit
-  LibraryPlaylistSortProperties 

Protocol

# LibraryPlaylistSortProperties

Playlist properties your app uses to sort results for a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol LibraryPlaylistSortProperties
```

## Topics

### Instance Properties

var lastPlayedDate: Date?

The date when the user last played the playlist on this device.

**Required**

var libraryAddedDate: Date?

The date when the user added the playlist to the library.

**Required**

var name: String

The name of the playlist.

**Required**

