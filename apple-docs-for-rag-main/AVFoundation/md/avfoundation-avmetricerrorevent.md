

- AVFoundation
-  AVMetricErrorEvent 

Class

# AVMetricErrorEvent

An object that represents a metric event when an error occurs.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class AVMetricErrorEvent
```

## Topics

### Getting the error

var error: any Error

Returns the error event.

var didRecover: Bool

A Boolean value that indicates whether the error was recoverable.

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

### Metrics

struct AVMetrics

An asynchronous stream of metric information.

struct AVMergedMetrics

An asynchronous stream of metric information from different publishers.

class AVVideoPerformanceMetrics

An object that provides metrics related to video playback quality.

protocol AVMetricEventStreamPublisher

A type for objects that publish metric events to the event stream.

class AVMetricEvent

A base class that represents a metric event.

Metric event types

