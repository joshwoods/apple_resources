

- AVFoundation
-  AVPlayerItemIntegratedTimelineObserver 

Protocol

# AVPlayerItemIntegratedTimelineObserver

A protocol for objects that perform timeline observations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVPlayerItemIntegratedTimelineObserver : NSObjectProtocol
```

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Observing time changes

func periodicTimes(forInterval: CMTime) -> AVPlayerItemIntegratedTimeline.PeriodicTimes

Returns an asynchronous sequence of times periodically as playback progresses.

func boundaryTimes(for: AVPlayerItemSegment, offsetsIntoSegment: [CMTime]) -> AVPlayerItemIntegratedTimeline.BoundaryTimes

Returns an asynchronous sequence of times whenever playback reaches a segment time in the segment.

struct BoundaryTimes

An asynchronous sequence of boundary time values.

struct PeriodicTimes

An asynchronous sequence of periodic time values.

