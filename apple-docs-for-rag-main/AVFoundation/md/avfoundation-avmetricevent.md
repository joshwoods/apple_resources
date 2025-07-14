

- AVFoundation
-  AVMetricEvent 

Class

# AVMetricEvent

A base class that represents a metric event.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVMetricEvent
```

## Topics

### Inspecting an event

var date: Date

var mediaTime: CMTime

var sessionID: String?

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMetricContentKeyRequestEvent
- AVMetricErrorEvent
- AVMetricHLSMediaSegmentRequestEvent
- AVMetricHLSPlaylistRequestEvent
- AVMetricMediaResourceRequestEvent
- AVMetricPlayerItemLikelyToKeepUpEvent
- AVMetricPlayerItemPlaybackSummaryEvent
- AVMetricPlayerItemRateChangeEvent
- AVMetricPlayerItemVariantSwitchEvent
- AVMetricPlayerItemVariantSwitchStartEvent

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

### Metrics

struct AVMetrics

An asynchronous stream of metric information.

struct AVMergedMetrics

An asynchronous stream of metric information from different publishers.

class AVVideoPerformanceMetrics

An object that provides metrics related to video playback quality.

protocol AVMetricEventStreamPublisher

A type for objects that publish metric events to the event stream.

class AVMetricErrorEvent

An object that represents a metric event when an error occurs.

Metric event types

