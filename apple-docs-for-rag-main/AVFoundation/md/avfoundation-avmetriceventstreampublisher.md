

- AVFoundation
-  AVMetricEventStreamPublisher 

Protocol

# AVMetricEventStreamPublisher

A type for objects that publish metric events to the event stream.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol AVMetricEventStreamPublisher
```

## Topics

### Getting the metrics

func allMetrics() -> AVMetrics&lt;AVMetricEvent>

func metrics&lt;MetricEvent>(forType: MetricEvent.Type) -> AVMetrics&lt;MetricEvent>

## Relationships

### Conforming Types

- AVPlayerItem

## See Also

### Metrics

struct AVMetrics

An asynchronous stream of metric information.

struct AVMergedMetrics

An asynchronous stream of metric information from different publishers.

class AVVideoPerformanceMetrics

An object that provides metrics related to video playback quality.

class AVMetricEvent

A base class that represents a metric event.

class AVMetricErrorEvent

An object that represents a metric event when an error occurs.

Metric event types

