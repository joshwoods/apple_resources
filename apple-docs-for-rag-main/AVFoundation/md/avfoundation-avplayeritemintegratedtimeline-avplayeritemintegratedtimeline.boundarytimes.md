

- AVFoundation
- AVPlayerItemIntegratedTimeline
-  AVPlayerItemIntegratedTimeline.BoundaryTimes 

Structure

# AVPlayerItemIntegratedTimeline.BoundaryTimes

An asynchronous sequence of boundary time values.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct BoundaryTimes
```

## Topics

### Iterating elements

struct Iterator

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Observing time changes

func periodicTimes(forInterval: CMTime) -> AVPlayerItemIntegratedTimeline.PeriodicTimes

Returns an asynchronous sequence of times periodically as playback progresses.

func boundaryTimes(for: AVPlayerItemSegment, offsetsIntoSegment: [CMTime]) -> AVPlayerItemIntegratedTimeline.BoundaryTimes

Returns an asynchronous sequence of times whenever playback reaches a segment time in the segment.

struct PeriodicTimes

An asynchronous sequence of periodic time values.

protocol AVPlayerItemIntegratedTimelineObserver

A protocol for objects that perform timeline observations.

