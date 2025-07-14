

- AVFoundation
- AVPlayer
-  init(url:) 

Initializer

# init(url:)

Creates a new player to play a single audiovisual resource referenced by a given URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
init(url URL: URL)
```

## Parameters 

`URL`  

A URL that identifies an audiovisual resource.

## Return Value

A new player instance initialized to play the audiovisual resource specified by `URL`.

## Discussion

This method implicitly creates an AVPlayerItem object. You can get the player item using currentItem.

## See Also

### Creating a Player

init(playerItem: AVPlayerItem?)

Creates a new player to play the specified player item.

init()

Creates a player object.

