

- Media Player
- MPMediaItem
-  lastPlayedDate 

Instance Property

# lastPlayedDate

The most recent play date of the media item.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
var lastPlayedDate: Date? { get }
```

## See Also

### Media item properties

var albumArtist: String?

The primary performing artist for an album.

var albumArtistPersistentID: MPMediaEntityPersistentID

The persistent identifier for the primary performing artist for an album.

var albumPersistentID: MPMediaEntityPersistentID

The persistent identifier for an album.

var albumTitle: String?

The title of an album, such as *Live on Mars*, rather than the title of an individual song on the album, such as “Crater Dance.”

var albumTrackCount: Int

The number of tracks for the album that contains the media item.

var albumTrackNumber: Int

The track number of the media item, for a media item that’s part of an album.

var artist: String?

The performing artists for a media item, which may vary from the primary artist for the album that a media item belongs to.

var artistPersistentID: MPMediaEntityPersistentID

The persistent identifier for an artist.

var artwork: MPMediaItemArtwork?

The artwork image for the media item.

var assetURL: URL?

The URL that points to the media item.

var beatsPerMinute: Int

The number of musical beats per minute for the media item.

var bookmarkTime: TimeInterval

The time of the user’s most recent interaction with the bookmark in the media item.

var isCloudItem: Bool

A Boolean value that indicates whether the media item is an iCloud Music Library item.

var comments: String?

Textual information about the media item.

var isCompilation: Bool

A Boolean value that indicates whether the media item is part of a compilation.

