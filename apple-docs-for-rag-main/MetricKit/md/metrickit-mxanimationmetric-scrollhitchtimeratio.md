

- MetricKit
- MXAnimationMetric
-  scrollHitchTimeRatio 

Instance Property

# scrollHitchTimeRatio

The ratio of the time spent hitching while scrolling.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var scrollHitchTimeRatio: Measurement { get }
```

## Discussion

Hitches are user-perceivable animation issues, such as pauses or jumps that occur during scrolling.

Note

This metric applies only to scrolling in UIScrollView.

