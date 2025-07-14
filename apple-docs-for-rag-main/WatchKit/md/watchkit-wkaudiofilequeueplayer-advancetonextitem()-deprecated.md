

- WatchKit
- WKAudioFileQueuePlayer
-  advanceToNextItem() Deprecated

Instance Method

# advanceToNextItem()

Ends playback of the current item and begins playing the next item in the queue.

watchOS 2.0–6.0Deprecated

``` source
func advanceToNextItem()
```

## Discussion

The method removes the current item from the queue before beginning playback of the next item.

## See Also

### Managing Items

var items: [WKAudioFilePlayerItem]

The array of queued items.

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

