

- AVFoundation
- AVPlayer
-  init(playerItem:) 

Initializer

# init(playerItem:)

Creates a new player to play the specified player item.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
init(playerItem item: AVPlayerItem?)
```

## Parameters 

`item`  

The player item to play.

## Return Value

A new player initialized to play `item`.

## See Also

### Creating a Player

init(url: URL)

Creates a new player to play a single audiovisual resource referenced by a given URL.

init()

Creates a player object.

