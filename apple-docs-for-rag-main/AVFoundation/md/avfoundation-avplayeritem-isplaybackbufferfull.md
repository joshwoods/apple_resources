

- AVFoundation
- AVPlayerItem
-  isPlaybackBufferFull 

Instance Property

# isPlaybackBufferFull

A Boolean value that indicates whether the internal media buffer is full and that further I/O is suspended.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
var isPlaybackBufferFull: Bool { get }
```

## Discussion

Despite the playback buffer reaching capacity there might not exist sufficient statistical data to support a isPlaybackLikelyToKeepUp prediction of true.

## See Also

### Determining Buffering Status

var isPlaybackLikelyToKeepUp: Bool

A Boolean value that indicates whether the item will likely play through without stalling.

var isPlaybackBufferEmpty: Bool

A Boolean value that indicates whether playback has consumed all buffered media and that playback will stall or end.

