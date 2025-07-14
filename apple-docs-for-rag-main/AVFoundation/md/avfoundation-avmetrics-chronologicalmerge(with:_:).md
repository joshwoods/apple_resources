

- AVFoundation
- AVMetrics
-  chronologicalMerge(with:\_:) 

Instance Method

# chronologicalMerge(with:\_:)

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func chronologicalMerge(
    with secondMetric: AVMetrics,
    _ metrics: repeat AVMetrics
) -> AVMergedMetrics where OtherSecondMetric : AVMetricEvent, repeat each MetricEventPack : AVMetricEvent
```

