

- AVFoundation
-  AVMetricMediaResourceRequestEvent 

Class

# AVMetricMediaResourceRequestEvent

An event that represents a media resource request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVMetricMediaResourceRequestEvent
```

## Topics

### Inspecting the event

var byteRange: NSRange

var errorEvent: AVMetricErrorEvent?

var networkTransactionMetrics: URLSessionTaskMetrics?

var requestEndTime: Date

var requestStartTime: Date

var responseEndTime: Date

var responseStartTime: Date

var serverAddress: String?

var url: URL?

var wasReadFromCache: Bool

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

### HTTP Live Streaming

class AVMetricContentKeyRequestEvent

An event that represents a live streaming content key resource request.

class AVMetricHLSMediaSegmentRequestEvent

An event that represents a live streaming media segment resource request.

class AVMetricHLSPlaylistRequestEvent

An event that represents a live streaming playlist resource request.

class AVMetricPlayerItemVariantSwitchStartEvent

An event that represents when the player attempts a variant switch.

class AVMetricPlayerItemVariantSwitchEvent

An event that represents when the player completes a variant switch.

