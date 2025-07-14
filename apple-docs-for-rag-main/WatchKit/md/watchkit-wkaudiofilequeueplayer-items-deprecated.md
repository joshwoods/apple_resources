

- WatchKit
- WKAudioFileQueuePlayer
-  items Deprecated

Instance Property

# items

The array of queued items.

watchOS 2.0–6.0Deprecated

``` source
var items: [WKAudioFilePlayerItem] { get }
```

## Discussion

This property contains the array of queued WKAudioFilePlayerItem objects. The initial contents of this array are set at initialization time but you may add or remove items using the methods of this class.

## See Also

### Managing Items

func advanceToNextItem()

Ends playback of the current item and begins playing the next item in the queue.

Deprecated

func appendItem(WKAudioFilePlayerItem)

Adds the specified item to the end of the queue.

Deprecated

func removeItem(WKAudioFilePlayerItem)

Removes the specified item from the queue.

Deprecated

func removeAllItems()

Removes all items from the queue.

Deprecated

