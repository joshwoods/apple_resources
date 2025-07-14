

- AVFoundation
- AVPlayerItem
-  forwardPlaybackEndTime 

Instance Property

# forwardPlaybackEndTime

The time at which forward playback ends.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
var forwardPlaybackEndTime: CMTime { get set }
```

## Discussion

The value indicates the time at which playback should end when the playback rate is positive (see `AVPlayer`’s rate property).

The default value is invalid, which indicates that no end time for forward playback is specified. In this case, the effective end time for forward playback is the item’s duration.

The value of this property has no effect on playback when the rate is negative.

## See Also

### Setting Playback Boundaries

var reversePlaybackEndTime: CMTime

The time at which reverse playback ends.

