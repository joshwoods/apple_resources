

- WatchKit
- WKAudioFileQueuePlayer
-  init(items:) Deprecated

Initializer

# init(items:)

Creates and returns a player initialized with an array of items.

watchOS 2.0–6.0Deprecated

``` source
convenience init(items: [WKAudioFilePlayerItem])
```

## Parameters 

`items`  

An array of WKAudioFilePlayerItem objects representing the assets to play. The order of the objects queue corresponds to the playback order of the assets.

## Return Value

An initialized player object.

## Discussion

The contents of the `items` property represent the initial items to play but you may add items to this queue later.

