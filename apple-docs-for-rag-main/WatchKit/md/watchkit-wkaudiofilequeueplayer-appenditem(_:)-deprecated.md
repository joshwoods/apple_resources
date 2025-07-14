

- WatchKit
- WKAudioFileQueuePlayer
-  appendItem(\_:) Deprecated

Instance Method

# appendItem(\_:)

Adds the specified item to the end of the queue.

watchOS 2.0–6.0Deprecated

``` source
func appendItem(_ item: WKAudioFilePlayerItem)
```

## Parameters 

`item`  

The player item to add to the queue.

## See Also

### Managing Items

var items: [WKAudioFilePlayerItem]

The array of queued items.

Deprecated

func advanceToNextItem()

Ends playback of the current item and begins playing the next item in the queue.

Deprecated

func removeItem(WKAudioFilePlayerItem)

Removes the specified item from the queue.

Deprecated

func removeAllItems()

Removes all items from the queue.

Deprecated

