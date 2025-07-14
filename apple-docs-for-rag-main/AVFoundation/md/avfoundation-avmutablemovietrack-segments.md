

- AVFoundation
- AVMutableMovieTrack
-  segments 

Instance Property

# segments

The time mappings from the track’s media samples to its timeline.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var segments: [AVAssetTrackSegment] { get }
```

## See Also

### Accessing Track Segments

func segment(forTrackTime: CMTime) -> AVAssetTrackSegment?

Returns a segment whose target time range contains, or is closest to, the specified track time.

