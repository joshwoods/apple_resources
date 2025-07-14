

- AVFoundation
- AVCompositionTrackSegment
-  init(timeRange:) 

Initializer

# init(timeRange:)

Creates an object that presents an empty composition track segment.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(timeRange: CMTimeRange)
```

## Parameters 

`timeRange`  

The time range of the empty track segment.

## See Also

### Creating a Segment

init(url: URL, trackID: CMPersistentTrackID, sourceTimeRange: CMTimeRange, targetTimeRange: CMTimeRange)

Creates an object that presents a segment of a media file that the specified URL references.

