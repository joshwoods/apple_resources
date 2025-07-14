

- AVFoundation
- AVCompositionTrackSegment
-  isEmpty 

Instance Property

# isEmpty

A Boolean value that indicates whether the segment is empty.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var isEmpty: Bool { get }
```

## Discussion

An empty segment has a valid target time range, but its sourceURL value is `nil` and the source start time is invalid. It doesn’t set values for its other properties.

## See Also

### Accessing Segment Properties

var sourceURL: URL?

A URL of the container file whose media this track segment presents.

var sourceTrackID: CMPersistentTrackID

An identifier of a track in the container file whose media this track segment presents.

