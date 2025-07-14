

- AVFoundation
-  AVVideoPerformanceMetrics 

Class

# AVVideoPerformanceMetrics

An object that provides metrics related to video playback quality.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+

``` source
class AVVideoPerformanceMetrics
```

## Topics

### Inspecting metrics

var totalNumberOfFrames: Int

The total number of frames that display if no frames drop.

var numberOfDroppedFrames: Int

The total number of frames the system drops prior to decoding or from missing the display deadline.

var numberOfCorruptedFrames: Int

The total number of corrupted frames.

var numberOfFramesDisplayedUsingOptimizedCompositing: Int

The total number of full screen frames rendered in a special power-efficient mode that didn’t require compositing with other UI elements.

var totalAccumulatedFrameDelay: TimeInterval

The accumulated amount of time between the prescribed presentation times of displayed video frames and their actual time of display.

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

### Metrics

struct AVMetrics

An asynchronous stream of metric information.

struct AVMergedMetrics

An asynchronous stream of metric information from different publishers.

protocol AVMetricEventStreamPublisher

A type for objects that publish metric events to the event stream.

class AVMetricEvent

A base class that represents a metric event.

class AVMetricErrorEvent

An object that represents a metric event when an error occurs.

Metric event types

