

- AVFoundation
- AVMutableMovie
-  providesPreciseDurationAndTiming 

Instance Property

# providesPreciseDurationAndTiming

A Boolean value that indicates whether the asset provides precise duration and timing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var providesPreciseDurationAndTiming: Bool { get }
```

## Discussion

This property value is true if you initialized the asset with the AVURLAssetPreferPreciseDurationAndTimingKey initialization option, otherwise it’s false.

## See Also

### Accessing Duration and Timing

var duration: CMTime

A time value that indicates the asset’s duration.

var minimumTimeOffsetFromLive: CMTime

A time value that indicates how closely playback follows the latest live stream content.

