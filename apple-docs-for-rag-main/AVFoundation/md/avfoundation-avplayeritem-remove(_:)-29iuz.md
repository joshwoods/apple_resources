

- AVFoundation
- AVPlayerItem
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the specified media data collector from the player item’s collection of media collectors.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.3+tvOS 9.2+visionOS 1.0+watchOS 2.3+

``` source
nonisolated
func remove(_ collector: AVPlayerItemMediaDataCollector)
```

## Parameters 

`collector`  

The instance of AVPlayerItemMediaDataCollector to remove.

## See Also

### Managing Player Item Data Collectors

var mediaDataCollectors: [AVPlayerItemMediaDataCollector]

The collection of associated media data collectors.

func add(AVPlayerItemMediaDataCollector)

Adds the specified media data collector to the player item’s collection of media collectors.

