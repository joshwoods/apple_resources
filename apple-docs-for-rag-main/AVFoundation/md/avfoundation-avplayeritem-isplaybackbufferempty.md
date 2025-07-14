

- AVFoundation
- AVPlayerItem
-  isPlaybackBufferEmpty 

Instance Property

# isPlaybackBufferEmpty

A Boolean value that indicates whether playback has consumed all buffered media and that playback will stall or end.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
var isPlaybackBufferEmpty: Bool { get }
```

## See Also

### Determining Buffering Status

var isPlaybackLikelyToKeepUp: Bool

A Boolean value that indicates whether the item will likely play through without stalling.

var isPlaybackBufferFull: Bool

A Boolean value that indicates whether the internal media buffer is full and that further I/O is suspended.

