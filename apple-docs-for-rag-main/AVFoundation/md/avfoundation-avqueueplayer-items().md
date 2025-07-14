

- AVFoundation
- AVQueuePlayer
-  items() 

Instance Method

# items()

Returns an array of the currently enqueued items.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func items() -> [AVPlayerItem]
```

## Return Value

An array of the currently enqueued player items.

## Discussion

The array contains AVPlayerItem objects currently in the player’s queue.

## See Also

### Managing the Player Queue

func advanceToNextItem()

Ends playback of the current item and starts playback of the next item in the player’s queue.

func canInsert(AVPlayerItem, after: AVPlayerItem?) -> Bool

Returns a Boolean value that indicates whether you can insert a player item into the player’s queue.

func insert(AVPlayerItem, after: AVPlayerItem?)

Inserts a player item after another player item in the queue.

func remove(AVPlayerItem)

Removes a given player item from the queue.

func removeAllItems()

Removes all player items from the queue.

