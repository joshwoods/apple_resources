

- ShazamKit
- SHMediaItem
-  artist 

Instance Property

# artist

The name of the artist for the media item, such as the performer of a song.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var artist: String? { get }
```

## See Also

### Reading general media item properties

var title: String?

A title for the media item.

var subtitle: String?

A subtitle for the media item.

var artworkURL: URL?

The URL for artwork for the media item, such as an album cover.

var videoURL: URL?

The URL for a video for the media item, such as a music video.

var genres: [String]

An array of genre names for the media item.

var explicitContent: Bool

A Boolean value that indicates whether the media item contains explicit content.

var creationDate: Date?

The date the media item was created.

var isrc: String?

The International Standard Recording Code (ISRC) for the media item.

var id: UUID

A unique identifier for this media item.

