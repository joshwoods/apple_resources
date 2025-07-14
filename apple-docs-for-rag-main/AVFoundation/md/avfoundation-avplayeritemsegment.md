

- AVFoundation
-  AVPlayerItemSegment 

Class

# AVPlayerItemSegment

An immutable object that represents a segment of time on the integrated timeline.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVPlayerItemSegment
```

## Topics

### Identifying the type

var segmentType: AVPlayerItemSegment.SegmentType

The type content this segment represents.

enum SegmentType

Constants that specify the type of segment.

### Inspecting the segment

var timeMapping: CMTimeMapping

The time mapping for this segment.

var loadedTimeRanges: [CMTimeRange]

The time ranges for the segment that have media data is readily available.

var startDate: Date?

The date at which a segment starts.

var interstitialEvent: AVPlayerInterstitialEvent?

The associated interstitial event for this segment.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Inspecting the snapshot

var duration: CMTime

The total duration of the primary item and scheduled interstitial events.

var currentSegment: AVPlayerItemSegment?

The currently playing segment.

var segments: [AVPlayerItemSegment]

The segments for this snapshot.

var currentTime: CMTime

The current time on the integrated timeline when the system created the snapshot.

var currentDate: Date?

The current date on the integrated timeline when the system created the snapshot.

