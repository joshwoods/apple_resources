

- AVFoundation
-  AVMovieTrack 

Class

# AVMovieTrack

A track in a movie that conforms to the QuickTime or ISO base media file format.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
class AVMovieTrack
```

## Topics

### Retrieving Track Information

var alternateGroupID: Int

A value that identifies the track as a member of a particular alternate group.

var mediaDataStorage: AVMediaDataStorage?

The storage container for media data added to a track.

var mediaDecodeTimeRange: CMTimeRange

A range of decode times for the track’s media.

var mediaPresentationTimeRange: CMTimeRange

A range of presentation times for the track’s media.

## Relationships

### Inherits From

- AVAssetTrack

### Inherited By

- AVFragmentedMovieTrack
- AVMutableMovieTrack

### Conforms To

- AVAsynchronousKeyValueLoading
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Movies

class AVMovie

An object that represents an audiovisual container that conforms to the QuickTime movie file format or a related format like MPEG-4.

