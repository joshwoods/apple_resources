

- MusicKit
-  LibraryMusicVideoSortProperties 

Protocol

# LibraryMusicVideoSortProperties

Music video properties your app uses to sort results for a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol LibraryMusicVideoSortProperties
```

## Topics

### Instance Properties

var albumTitle: String?

The title of the album the music video appears on.

**Required**

var artistName: String?

The artist’s name.

**Required**

var duration: TimeInterval?

The duration of the music video.

**Required**

var lastPlayedDate: Date?

The date when the user last played the music video on this device.

**Required**

var libraryAddedDate: Date?

The date when the user added the music video to the library.

**Required**

var playCount: Int?

The number of times the user played the music video.

**Required**

var title: String

The title of the music video.

**Required**

var trackNumber: Int?

The music video’s number in the album’s track list.

**Required**

