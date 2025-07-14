

- AVFoundation
- AVQueuePlayer
-  canInsert(\_:after:) 

Instance Method

# canInsert(\_:after:)

Returns a Boolean value that indicates whether you can insert a player item into the player’s queue.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func canInsert(
    _ item: AVPlayerItem,
    after afterItem: AVPlayerItem?
) -> Bool
```

## Parameters 

`item`  

The player item to insert.

`afterItem`  

The player item in the queue to follow. Pass `nil` to test if you can append the item to the queue.

## Return Value

true if `item` can be appended to the queue, otherwise false.

## Discussion

Adding the same item to a player at more than one position in the queue isn’t supported.

## See Also

### Managing the Player Queue

func items() -> [AVPlayerItem]

Returns an array of the currently enqueued items.

func advanceToNextItem()

Ends playback of the current item and starts playback of the next item in the player’s queue.

func insert(AVPlayerItem, after: AVPlayerItem?)

Inserts a player item after another player item in the queue.

func remove(AVPlayerItem)

Removes a given player item from the queue.

func removeAllItems()

Removes all player items from the queue.

