

- AVFoundation
- AVMutableMovie
-  minimumTimeOffsetFromLive 

Instance Property

# minimumTimeOffsetFromLive

A time value that indicates how closely playback follows the latest live stream content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
var minimumTimeOffsetFromLive: CMTime { get }
```

## Discussion

This property value is only valid when working with live streaming content. For non-live assets, this property value is invalid.

## See Also

### Accessing Duration and Timing

var duration: CMTime

A time value that indicates the asset’s duration.

var providesPreciseDurationAndTiming: Bool

A Boolean value that indicates whether the asset provides precise duration and timing.

