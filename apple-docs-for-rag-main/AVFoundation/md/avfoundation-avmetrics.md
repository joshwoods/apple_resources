

- AVFoundation
-  AVMetrics 

Structure

# AVMetrics

An asynchronous stream of metric information.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct AVMetrics where MetricEvent : AVMetricEvent
```

## Topics

### Merging metrics

func chronologicalMerge&lt;OtherSecondMetric, each MetricEventPack>(with: AVMetrics&lt;OtherSecondMetric>, repeat AVMetrics&lt;each MetricEventPack>) -> AVMergedMetrics&lt;MetricEvent, OtherSecondMetric, repeat each MetricEventPack>

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Metrics

struct AVMergedMetrics

An asynchronous stream of metric information from different publishers.

class AVVideoPerformanceMetrics

An object that provides metrics related to video playback quality.

protocol AVMetricEventStreamPublisher

A type for objects that publish metric events to the event stream.

class AVMetricEvent

A base class that represents a metric event.

class AVMetricErrorEvent

An object that represents a metric event when an error occurs.

Metric event types

