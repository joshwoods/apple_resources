

- AVFoundation
- AVCompositionTrack
-  segments 

Instance Property

# segments

The time mappings from the track’s media samples to its timeline.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var segments: [AVCompositionTrackSegment] { get }
```

## See Also

### Accessing Track Segments

func segment(forTrackTime: CMTime) -> AVCompositionTrackSegment?

Returns a segment whose target time range contains, or is closest to, the specified track time.

