

- AVFoundation
- AVPlayerItem
-  seekableTimeRanges 

Instance Property

# seekableTimeRanges

An array of time ranges within which it is possible to seek.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
var seekableTimeRanges: [NSValue] { get }
```

## Discussion

The array contains NSValue objects containing a CMTimeRange value indicating the times ranges to which the player item can seek. The time ranges returned may be discontinuous.

## See Also

### Determining Available Time Ranges

var loadedTimeRanges: [NSValue]

An array of time ranges indicating media data that is readily available.

