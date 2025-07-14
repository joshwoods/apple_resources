

- AVFoundation
- AVPlayer
-  rate 

Instance Property

# rate

The current playback rate.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
var rate: Float { get set }
```

## Mentioned in 

Controlling the transport behavior of a player

## See Also

### Controlling Playback

var defaultRate: Float

A default rate at which to begin playback.

func play()

Begins playback of the current item.

func pause()

Pauses playback of the current item.

class let rateDidChangeNotification: NSNotification.Name

A notification that a player posts when its rate changes.

