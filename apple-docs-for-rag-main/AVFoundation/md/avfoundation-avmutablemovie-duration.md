

- AVFoundation
- AVMutableMovie
-  duration 

Instance Property

# duration

A time value that indicates the asset’s duration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var duration: CMTime { get }
```

## Discussion

If you initialized the composition’s assets by passing the AVURLAssetPreferPreciseDurationAndTimingKey initialization option, this property value provides precise duration; otherwise, it provides a best-available estimate. You can determine the value’s accuracy by querying the asset’s providesPreciseDurationAndTiming property.

## See Also

### Accessing Duration and Timing

var providesPreciseDurationAndTiming: Bool

A Boolean value that indicates whether the asset provides precise duration and timing.

var minimumTimeOffsetFromLive: CMTime

A time value that indicates how closely playback follows the latest live stream content.

