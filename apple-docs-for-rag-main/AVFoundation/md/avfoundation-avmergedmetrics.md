

- AVFoundation
-  AVMergedMetrics 

Structure

# AVMergedMetrics

An asynchronous stream of metric information from different publishers.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct AVMergedMetrics where MetricEvent1 : AVMetricEvent, MetricEvent2 : AVMetricEvent, repeat each MetricEventPack : AVMetricEvent
```

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Metrics

struct AVMetrics

An asynchronous stream of metric information.

class AVVideoPerformanceMetrics

An object that provides metrics related to video playback quality.

protocol AVMetricEventStreamPublisher

A type for objects that publish metric events to the event stream.

class AVMetricEvent

A base class that represents a metric event.

class AVMetricErrorEvent

An object that represents a metric event when an error occurs.

Metric event types

