

- AVFoundation
-  AVMetricPlayerItemSeekDidCompleteEvent 

Class

# AVMetricPlayerItemSeekDidCompleteEvent

An event that represents when the playback seek completes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVMetricPlayerItemSeekDidCompleteEvent
```

## Topics

### Inspecting the event

var didSeekInBuffer: Bool

## Relationships

### Inherits From

- AVMetricPlayerItemRateChangeEvent

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

class AVMetricPlayerItemRateChangeEvent

An event that represents when the playback rate changes.

class AVMetricPlayerItemSeekEvent

An event that represents when a playback seek occurs.

