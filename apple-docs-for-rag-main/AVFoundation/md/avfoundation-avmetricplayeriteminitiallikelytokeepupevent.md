

- AVFoundation
-  AVMetricPlayerItemInitialLikelyToKeepUpEvent 

Class

# AVMetricPlayerItemInitialLikelyToKeepUpEvent

An event that represents the initial state for whether playback is likely to continue without stalling.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVMetricPlayerItemInitialLikelyToKeepUpEvent
```

## Topics

### Inspecting the event

var contentKeyRequestEvents: [AVMetricContentKeyRequestEvent]

var mediaSegmentRequestEvents: [AVMetricHLSMediaSegmentRequestEvent]

var playlistRequestEvents: [AVMetricHLSPlaylistRequestEvent]

## Relationships

### Inherits From

- AVMetricPlayerItemLikelyToKeepUpEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Buffering

class AVMetricPlayerItemStallEvent

An event that represents when playback stalls.

class AVMetricPlayerItemLikelyToKeepUpEvent

An event that represents when playback is likely to continue without stalling.

