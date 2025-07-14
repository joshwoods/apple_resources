

- AVFoundation
- AVPlayerItemIntegratedTimeline
-  boundaryTimes(for:offsetsIntoSegment:) 

Instance Method

# boundaryTimes(for:offsetsIntoSegment:)

Returns an asynchronous sequence of times whenever playback reaches a segment time in the segment.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func boundaryTimes(
    for segment: AVPlayerItemSegment,
    offsetsIntoSegment: [CMTime]
) -> AVPlayerItemIntegratedTimeline.BoundaryTimes
```

## See Also

### Observing time changes

func periodicTimes(forInterval: CMTime) -> AVPlayerItemIntegratedTimeline.PeriodicTimes

Returns an asynchronous sequence of times periodically as playback progresses.

struct BoundaryTimes

An asynchronous sequence of boundary time values.

struct PeriodicTimes

An asynchronous sequence of periodic time values.

protocol AVPlayerItemIntegratedTimelineObserver

A protocol for objects that perform timeline observations.

