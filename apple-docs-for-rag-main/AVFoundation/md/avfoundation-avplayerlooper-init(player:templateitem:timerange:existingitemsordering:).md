

- AVFoundation
- AVPlayerLooper
-  init(player:templateItem:timeRange:existingItemsOrdering:) 

Initializer

# init(player:templateItem:timeRange:existingItemsOrdering:)

Creates a player looper that continuously plays the full duration of a player item while adhering to the specified ordering of existing items in the queue.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    player: AVQueuePlayer,
    templateItem itemToLoop: AVPlayerItem,
    timeRange loopRange: CMTimeRange,
    existingItemsOrdering itemOrdering: AVPlayerLooper.ItemOrdering
)
```

## Parameters 

`player`  

A queue player to control playback.

`itemToLoop`  

A player item to loop.

`loopRange`  

The player item time range to loop. Passing a value of invalid is equivalent to a time range of \[0, player item’s duration\].

`itemOrdering`  

A value that indicates whether the looper inserts replica items before or after existing items in the specified queue player.

## Discussion

The player looper doesn’t use the player item you specify for playback, and instead uses it as a template to create at least three player item replicas that it uses for looping playback. Because the looper only uses the player item as a template, any changes that you make to it after initialization aren’t reflected in the looping playback.

Important

Load the duration value of a player item’s asset before passing the item to the looper to prevent blocking the calling thread until the duration is known.

## Topics

### Item ordering

enum ItemOrdering

Constants that define the ordering of items in a player looper.

## See Also

### Creating a Player Looper

convenience init(player: AVQueuePlayer, templateItem: AVPlayerItem)

Creates a player looper that continuously plays the full duration of a player item.

convenience init(player: AVQueuePlayer, templateItem: AVPlayerItem, timeRange: CMTimeRange)

Creates a player looper that continuously plays the specified time range of a player item.

