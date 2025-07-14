

- AVFoundation
- AVPlayerLooper
-  init(player:templateItem:) 

Initializer

# init(player:templateItem:)

Creates a player looper that continuously plays the full duration of a player item.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
convenience init(
    player: AVQueuePlayer,
    templateItem itemToLoop: AVPlayerItem
)
```

## Parameters 

`player`  

The queue player to use for playback. The player must not be `nil`.

`itemToLoop`  

The player item to loop, which must not be `nil`.

## Return Value

An new instance of `AVPlayerLooper`.

## Discussion

Creating an instance of this class using this method is equivalent to calling init(player:templateItem:timeRange:) and passing a value of invalid for the `timeRange` parameter.

## See Also

### Creating a Player Looper

init(player: AVQueuePlayer, templateItem: AVPlayerItem, timeRange: CMTimeRange, existingItemsOrdering: AVPlayerLooper.ItemOrdering)

Creates a player looper that continuously plays the full duration of a player item while adhering to the specified ordering of existing items in the queue.

convenience init(player: AVQueuePlayer, templateItem: AVPlayerItem, timeRange: CMTimeRange)

Creates a player looper that continuously plays the specified time range of a player item.

