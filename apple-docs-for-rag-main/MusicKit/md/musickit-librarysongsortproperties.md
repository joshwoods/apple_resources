

- MusicKit
-  LibrarySongSortProperties 

Protocol

# LibrarySongSortProperties

Song properties your app uses to sort results for a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol LibrarySongSortProperties
```

## Topics

### Instance Properties

var albumTitle: String?

The title of the album the song appears on.

**Required**

var artistName: String?

The artist’s name.

**Required**

var composerName: String?

The name of the song’s composer.

**Required**

var discNumber: Int?

The disc number of the song.

**Required**

var duration: TimeInterval?

The duration of the song.

**Required**

var lastPlayedDate: Date?

The date when the user last played the song on this device.

**Required**

var libraryAddedDate: Date?

The date when the user added the song to the library.

**Required**

var playCount: Int?

The number of times the user played the song.

**Required**

var title: String

The title of the song.

**Required**

var trackNumber: Int?

The song’s number in the album’s track list.

**Required**

