

- AVFoundation
-  AVCompositionTrackSegment 

Class

# AVCompositionTrackSegment

A track segment that maps a time from the source media track to the composition track.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVCompositionTrackSegment
```

## Overview

You typically use this class to save a low-level representation of a composition.

## Topics

### Creating a Segment

init(timeRange: CMTimeRange)

Creates an object that presents an empty composition track segment.

init(url: URL, trackID: CMPersistentTrackID, sourceTimeRange: CMTimeRange, targetTimeRange: CMTimeRange)

Creates an object that presents a segment of a media file that the specified URL references.

### Accessing Segment Properties

var sourceURL: URL?

A URL of the container file whose media this track segment presents.

var sourceTrackID: CMPersistentTrackID

An identifier of a track in the container file whose media this track segment presents.

var isEmpty: Bool

A Boolean value that indicates whether the segment is empty.

## Relationships

### Inherits From

- AVAssetTrackSegment

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Compositions

class AVComposition

An object that combines and arranges media from multiple assets into a single composite asset that you can play or process.

class AVCompositionTrack

A track in a composition that presents media of a uniform type.

