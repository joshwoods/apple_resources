

- Vision
- VNObservation
-  timeRange 

Instance Property

# timeRange

The time range of the reported observation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var timeRange: CMTimeRange { get }
```

## Discussion

When evaluating a sequence of image buffers, use this property to determine each observation’s start time and duration. If a request doesn’t support time ranges, or the time range is unknown, the value of this property is zero.

## See Also

### Evaluating Observations

var confidence: VNConfidence

The level of confidence in the observation’s accuracy.

typealias VNConfidence

A type alias for the confidence value of an observation.

