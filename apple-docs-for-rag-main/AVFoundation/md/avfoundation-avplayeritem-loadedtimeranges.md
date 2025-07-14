

- AVFoundation
- AVPlayerItem
-  loadedTimeRanges 

Instance Property

# loadedTimeRanges

An array of time ranges indicating media data that is readily available.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
var loadedTimeRanges: [NSValue] { get }
```

## Discussion

The array contains NSValue objects containing a CMTimeRange value indicating the times ranges for which the player item has media data readily available. The time ranges returned may be discontinuous.

## See Also

### Determining Available Time Ranges

var seekableTimeRanges: [NSValue]

An array of time ranges within which it is possible to seek.

