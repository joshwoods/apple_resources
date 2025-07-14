

- WatchKit
- WKAudioFileQueuePlayer
-  removeAllItems() Deprecated

Instance Method

# removeAllItems()

Removes all items from the queue.

watchOS 2.0–6.0Deprecated

``` source
func removeAllItems()
```

## Discussion

This method has the side effect of stopping playback.

## See Also

### Managing Items

var items: [WKAudioFilePlayerItem]

The array of queued items.

Deprecated

func advanceToNextItem()

Ends playback of the current item and begins playing the next item in the queue.

Deprecated

func appendItem(WKAudioFilePlayerItem)

Adds the specified item to the end of the queue.

Deprecated

func removeItem(WKAudioFilePlayerItem)

Removes the specified item from the queue.

Deprecated

