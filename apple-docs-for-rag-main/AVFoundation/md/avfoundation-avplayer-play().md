

- AVFoundation
- AVPlayer
-  play() 

Instance Method

# play()

Begins playback of the current item.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func play()
```

## Mentioned in 

Controlling the transport behavior of a player

## Discussion

Calling this method is the same as setting the rate to `1.0`.

Note

Before macOS 13, iOS 16, tvOS 16, and watchOS 9, you can only call this method on the main thread or queue.

## See Also

### Controlling Playback

var defaultRate: Float

A default rate at which to begin playback.

func pause()

Pauses playback of the current item.

var rate: Float

The current playback rate.

class let rateDidChangeNotification: NSNotification.Name

A notification that a player posts when its rate changes.

