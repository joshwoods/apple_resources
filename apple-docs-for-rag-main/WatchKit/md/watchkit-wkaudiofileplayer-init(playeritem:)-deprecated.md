

- WatchKit
- WKAudioFilePlayer
-  init(playerItem:) Deprecated

Initializer

# init(playerItem:)

Creates and returns a player initialized with the specified player item.

watchOS 2.0–6.0Deprecated

``` source
convenience init(playerItem item: WKAudioFilePlayerItem)
```

## Parameters 

`item`  

The player item containing the audio asset to play. This parameter must not be `nil`.

## Return Value

An initialized player object.

## See Also

### Creating a Player

func replaceCurrentItem(with: WKAudioFilePlayerItem?)

Replaces the current player item with a different one.

Deprecated

