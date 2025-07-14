

- MusicKit
-  LibraryTrackSortProperties 

Protocol

# LibraryTrackSortProperties

Track properties your app uses to sort results for a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol LibraryTrackSortProperties
```

## Topics

### Instance Properties

var albumTitle: String?

The title of the album the track appears on.

**Required**

var artistName: String?

The artist’s name.

**Required**

var discNumber: Int?

The disc number of the track.

**Required**

var duration: TimeInterval?

The duration of the track.

**Required**

var lastPlayedDate: Date?

The date when the user last played the track on this device.

**Required**

var libraryAddedDate: Date?

The date when the user added the track to the library.

**Required**

var playCount: Int?

The number of times the user played the track.

**Required**

var title: String

The title of the track.

**Required**

var trackNumber: Int?

The track’s number in the album’s track list.

**Required**

