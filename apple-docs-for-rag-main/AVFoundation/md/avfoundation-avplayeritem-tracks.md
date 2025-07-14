

- AVFoundation
- AVPlayerItem
-  tracks 

Instance Property

# tracks

An array of player item track objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
var tracks: [AVPlayerItemTrack] { get }
```

## Discussion

The value is an empty array before the player loads the underlying tracks. Key-value observe this property value to access valid tracks as soon as they’re available.

