

- AVFoundation
-  AVMetricPlayerItemLikelyToKeepUpEvent 

Class

# AVMetricPlayerItemLikelyToKeepUpEvent

An event that represents when playback is likely to continue without stalling.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVMetricPlayerItemLikelyToKeepUpEvent
```

## Topics

### Inspecting the event

var loadedTimeRanges: [CMTimeRange]

var timeTaken: TimeInterval

var variant: AVAssetVariant?

## Relationships

### Inherits From

- AVMetricEvent

### Inherited By

- AVMetricPlayerItemInitialLikelyToKeepUpEvent

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

class AVMetricPlayerItemInitialLikelyToKeepUpEvent

An event that represents the initial state for whether playback is likely to continue without stalling.

