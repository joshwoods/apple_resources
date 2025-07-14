

- WatchKit
- WKAudioFilePlayer
-  replaceCurrentItem(with:) Deprecated

Instance Method

# replaceCurrentItem(with:)

Replaces the current player item with a different one.

watchOS 2.0–6.0Deprecated

``` source
func replaceCurrentItem(with item: WKAudioFilePlayerItem?)
```

## Parameters 

`item`  

The player item whose contents you want to play.

## Discussion

The default implementation of this method does nothing. Subclasses can override it to implement support for swapping out the current player item for a new one.

## See Also

### Creating a Player

convenience init(playerItem: WKAudioFilePlayerItem)

Creates and returns a player initialized with the specified player item.

Deprecated

