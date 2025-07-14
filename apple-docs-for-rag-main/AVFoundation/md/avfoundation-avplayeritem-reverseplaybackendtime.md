

- AVFoundation
- AVPlayerItem
-  reversePlaybackEndTime 

Instance Property

# reversePlaybackEndTime

The time at which reverse playback ends.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
var reversePlaybackEndTime: CMTime { get set }
```

## Discussion

The value indicated the time at which playback should end when the playback rate is negative (see `AVPlayer`’s rate property).

The default value is invalid, which indicates that no end time for reverse playback is specified. In this case, the effective end time for reverse playback is zero.

The value of this property has no effect on playback when the rate is positive.

## See Also

### Setting Playback Boundaries

var forwardPlaybackEndTime: CMTime

The time at which forward playback ends.

