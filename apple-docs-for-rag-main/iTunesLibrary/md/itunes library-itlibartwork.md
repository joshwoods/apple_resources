

- iTunes Library
-  ITLibArtwork 

Class

# ITLibArtwork

This class represents the artwork for a media item.

Mac Catalyst 14.0+macOS 10.13+

``` source
class ITLibArtwork
```

## Topics

### Getting Artwork Info

var image: NSImage?

The artwork image.

var imageData: Data?

The raw image data of the artwork in the format that imageDataFormat specifies.

var imageDataFormat: ITLibArtworkFormat

The format of the artwork image data that imageData returns.

### Artwork Formats

enum ITLibArtworkFormat

These constants specify the possible formats of the data that imageDataFormat returns.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media Items

class ITLibMediaItem

This class describes a media item (a track) in the iTunes library, such as a song, a video, or a podcast.

class ITLibMediaEntity

This class describes a media entity, which can be a media item, such as an audio track.

class ITLibArtist

This class represents an artist, such as the performer of a song.

class ITLibMediaItemVideoInfo

This class encapsulates the video information of a video media item.

