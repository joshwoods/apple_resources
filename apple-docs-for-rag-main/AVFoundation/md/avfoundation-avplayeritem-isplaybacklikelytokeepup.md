

- AVFoundation
- AVPlayerItem
-  isPlaybackLikelyToKeepUp 

Instance Property

# isPlaybackLikelyToKeepUp

A Boolean value that indicates whether the item will likely play through without stalling.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
var isPlaybackLikelyToKeepUp: Bool { get }
```

## Discussion

This property communicates a prediction of playability. Factors considered in this prediction include I/O throughput and media decode performance. It is possible for `playbackLikelyToKeepUp` to indicate false while the property isPlaybackBufferFull indicates true. In this event the playback buffer has reached capacity but there isn’t the statistical data to support a prediction that playback is likely to keep up in the future. It is up to you to decide whether to continue media playback.

## See Also

### Determining Buffering Status

var isPlaybackBufferFull: Bool

A Boolean value that indicates whether the internal media buffer is full and that further I/O is suspended.

var isPlaybackBufferEmpty: Bool

A Boolean value that indicates whether playback has consumed all buffered media and that playback will stall or end.

