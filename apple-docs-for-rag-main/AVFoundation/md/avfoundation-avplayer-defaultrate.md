

- AVFoundation
- AVPlayer
-  defaultRate 

Instance Property

# defaultRate

A default rate at which to begin playback.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
var defaultRate: Float { get set }
```

## Mentioned in 

Controlling the transport behavior of a player

## Discussion

This value represents the default playback rate the player uses when you call its play() method. After playback begins, the rate may differ from the default if you modify the player’s rate value, such as by calling pause().

Important

Begin playback by calling the play() method. Don’t start playback by setting the rate property value to `1.0`. Instead, use rate to make immediate, temporary changes to the playback rate. The next time you call the play() method, the player restores the rate to the value of defaultRate.

## See Also

### Controlling Playback

func play()

Begins playback of the current item.

func pause()

Pauses playback of the current item.

var rate: Float

The current playback rate.

class let rateDidChangeNotification: NSNotification.Name

A notification that a player posts when its rate changes.

