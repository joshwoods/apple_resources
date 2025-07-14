

- AVFoundation
- AVPlayerItemIntegratedTimelineSnapshot
-  duration 

Instance Property

# duration

The total duration of the primary item and scheduled interstitial events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var duration: CMTime { get }
```

## Discussion

The duration property takes into account the interstitial event’s playoutLimit and resumptionOffset values.

Before loading the duration of the primary item, the value of this property is invalid. For livestreams, this value is indefinite.

## See Also

### Inspecting the snapshot

var currentSegment: AVPlayerItemSegment?

The currently playing segment.

var segments: [AVPlayerItemSegment]

The segments for this snapshot.

class AVPlayerItemSegment

An immutable object that represents a segment of time on the integrated timeline.

var currentTime: CMTime

The current time on the integrated timeline when the system created the snapshot.

var currentDate: Date?

The current date on the integrated timeline when the system created the snapshot.

