

- AVFoundation
- AVPlayerItemIntegratedTimelineSnapshot
-  currentSegment 

Instance Property

# currentSegment

The currently playing segment.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var currentSegment: AVPlayerItemSegment? { get }
```

## See Also

### Inspecting the snapshot

var duration: CMTime

The total duration of the primary item and scheduled interstitial events.

var segments: [AVPlayerItemSegment]

The segments for this snapshot.

class AVPlayerItemSegment

An immutable object that represents a segment of time on the integrated timeline.

var currentTime: CMTime

The current time on the integrated timeline when the system created the snapshot.

var currentDate: Date?

The current date on the integrated timeline when the system created the snapshot.

