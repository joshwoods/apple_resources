

- AVFoundation
- AVPlayer
-  pause() 

Instance Method

# pause()

Pauses playback of the current item.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func pause()
```

## Mentioned in 

Controlling the transport behavior of a player

## Discussion

Calling this method is the same as setting the rate to `0.0`.

## See Also

### Controlling Playback

var defaultRate: Float

A default rate at which to begin playback.

func play()

Begins playback of the current item.

var rate: Float

The current playback rate.

class let rateDidChangeNotification: NSNotification.Name

A notification that a player posts when its rate changes.

