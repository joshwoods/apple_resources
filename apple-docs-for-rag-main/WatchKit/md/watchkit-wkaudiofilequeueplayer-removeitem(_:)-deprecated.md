

- WatchKit
- WKAudioFileQueuePlayer
-  removeItem(\_:) Deprecated

Instance Method

# removeItem(\_:)

Removes the specified item from the queue.

watchOS 2.0–6.0Deprecated

``` source
func removeItem(_ item: WKAudioFilePlayerItem)
```

## Parameters 

`item`  

The player item to remove.

## Discussion

If `item` is currently playing, the queue stops playback of item before removing it. It then begins playing the next item in the queue.

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

func removeAllItems()

Removes all items from the queue.

Deprecated

