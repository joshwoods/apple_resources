

- AVFoundation
-  AVAssetTrackSegment 

Class

# AVAssetTrackSegment

An object that represents a time range segment of an asset track.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVAssetTrackSegment
```

## Topics

### Retrieving Segment Information

var timeMapping: CMTimeMapping

The time range of the track that this segment presents.

var isEmpty: Bool

A Boolean value that indicates whether the segment is empty.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVCompositionTrackSegment

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Assets

class AVAsset

An object that models timed audiovisual media.

class AVURLAsset

An asset that represents media at a local or remote URL.

class AVAssetTrack

An object that models a track of media that an asset contains.

class AVAssetTrackGroup

A group of related tracks in an asset.

