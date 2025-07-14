

- AVFoundation
- AVCompositionTrack
-  segment(forTrackTime:) 

Instance Method

# segment(forTrackTime:)

Returns a segment whose target time range contains, or is closest to, the specified track time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func segment(forTrackTime trackTime: CMTime) -> AVCompositionTrackSegment?
```

## Parameters 

`trackTime`  

The track time of the segment to return.

## Return Value

The AVCompositionTrackSegment associated with the track time.

## See Also

### Accessing Track Segments

var segments: [AVCompositionTrackSegment]

The time mappings from the track’s media samples to its timeline.

