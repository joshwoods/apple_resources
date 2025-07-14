

- AVFoundation
- AVPlayerItem
-  recommendedTimeOffsetFromLive 

Instance Property

# recommendedTimeOffsetFromLive

A recommended time offset from the live time based on observed network conditions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
var recommendedTimeOffsetFromLive: CMTime { get }
```

## Discussion

For nonlive stream content, the value is invalid.

## See Also

### Managing Time Offsets

var automaticallyPreservesTimeOffsetFromLive: Bool

A Boolean value that indicates whether the player preserves its time offset from the live time after a buffering operation.

var configuredTimeOffsetFromLive: CMTime

A time value that indicates the offset from the live time to start playback, or resume playback after a seek to positive infinity.

