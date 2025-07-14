

- AVFoundation
- AVCompositionTrack
-  requiresFrameReordering 

Instance Property

# requiresFrameReordering

A Boolean value that indicates whether samples in the track may have different presentation and decode timestamps.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var requiresFrameReordering: Bool { get }
```

## See Also

### Accessing Frame-Based Characteristics

var nominalFrameRate: Float

The frame rate of the track, in frames per second.

var minFrameDuration: CMTime

The minimum duration of the track’s frames.

