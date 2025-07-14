

- AVFoundation
- AVPlayer
-  replaceCurrentItem(with:) 

Instance Method

# replaceCurrentItem(with:)

Replaces the current item with a new item.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func replaceCurrentItem(with item: AVPlayerItem?)
```

## Parameters 

`item`  

The new item for the player object to play.

## Mentioned in 

Controlling the transport behavior of a player

## Discussion

The player item replacement occurs immediately and the item becomes the player’s currentItem. Calling this method with the player’s current player item has no effect.

## See Also

### Managing the Player Item

var currentItem: AVPlayerItem?

The item for which the player is currently controlling playback.

