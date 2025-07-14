

- AVFoundation
-  AVMetricPlayerItemPlaybackSummaryEvent 

Class

# AVMetricPlayerItemPlaybackSummaryEvent

An event that represents the combined metrics for the entire playback session.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVMetricPlayerItemPlaybackSummaryEvent
```

## Topics

### Inspecting the event

var errorEvent: AVMetricErrorEvent?

var mediaResourceRequestCount: Int

var playbackDuration: Int

var recoverableErrorCount: Int

var stallCount: Int

var timeSpentInInitialStartup: TimeInterval

var timeSpentRecoveringFromStall: TimeInterval

var timeWeightedAverageBitrate: Int

var timeWeightedPeakBitrate: Int

var variantSwitchCount: Int

## Relationships

### Inherits From

- AVMetricEvent

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

class AVMetricPlayerItemRateChangeEvent

An event that represents when the playback rate changes.

class AVMetricPlayerItemSeekDidCompleteEvent

An event that represents when the playback seek completes.

class AVMetricPlayerItemSeekEvent

An event that represents when a playback seek occurs.

