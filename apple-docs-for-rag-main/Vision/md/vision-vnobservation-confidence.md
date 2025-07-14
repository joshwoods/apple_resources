

- Vision
- VNObservation
-  confidence 

Instance Property

# confidence

The level of confidence in the observation’s accuracy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var confidence: VNConfidence { get }
```

## Discussion

The Vision framework normalizes this value to `[0.0, 1.0]` under most circumstances. A value of `0.0` indicates no confidence. A value of `1.0` indicates highest confidence, or the observation doesn’t support or assign meaning to confidence.

Note

When the results come from a VNCoreMLRequest, Vision forwards confidence values as-is and doesn’t normalize them.

## See Also

### Evaluating Observations

var timeRange: CMTimeRange

The time range of the reported observation.

typealias VNConfidence

A type alias for the confidence value of an observation.

