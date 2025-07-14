

- AVFoundation
-  AVMetricPlayerItemRateChangeEvent 

Class

# AVMetricPlayerItemRateChangeEvent

An event that represents when the playback rate changes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVMetricPlayerItemRateChangeEvent
```

## Topics

### Inspecting the event

var previousRate: Double

var rate: Double

var variant: AVAssetVariant?

## Relationships

### Inherits From

- AVMetricEvent

### Inherited By

- AVMetricPlayerItemSeekDidCompleteEvent
- AVMetricPlayerItemSeekEvent
- AVMetricPlayerItemStallEvent

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

### Transport control

class AVMetricPlayerItemPlaybackSummaryEvent

An event that represents the combined metrics for the entire playback session.

class AVMetricPlayerItemSeekDidCompleteEvent

An event that represents when the playback seek completes.

class AVMetricPlayerItemSeekEvent

An event that represents when a playback seek occurs.

