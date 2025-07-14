

- AVFoundation
- AVQueuePlayer
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes a given player item from the queue.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func remove(_ item: AVPlayerItem)
```

## Parameters 

`item`  

The player item to remove from the queue.

## Discussion

If the item is currently playing, calling this method has the same effect as calling the advanceToNextItem() method.

## See Also

### Managing the Player Queue

func items() -> [AVPlayerItem]

Returns an array of the currently enqueued items.

func advanceToNextItem()

Ends playback of the current item and starts playback of the next item in the player’s queue.

func canInsert(AVPlayerItem, after: AVPlayerItem?) -> Bool

Returns a Boolean value that indicates whether you can insert a player item into the player’s queue.

func insert(AVPlayerItem, after: AVPlayerItem?)

Inserts a player item after another player item in the queue.

func removeAllItems()

Removes all player items from the queue.

