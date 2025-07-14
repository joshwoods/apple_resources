

- AVFoundation
- AVComposition
-  providesPreciseDurationAndTiming 

Instance Property

# providesPreciseDurationAndTiming

A Boolean value that indicates whether the asset provides precise duration and timing.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

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

