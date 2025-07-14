

- AVFoundation
- AVQueuePlayer
-  removeAllItems() 

Instance Method

# removeAllItems()

Removes all player items from the queue.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
func removeAllItems()
```

## Discussion

Calling this method removes all currently enqueued player items and stops playback.

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

func remove(AVPlayerItem)

Removes a given player item from the queue.

