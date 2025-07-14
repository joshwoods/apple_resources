

- AVKit
- VideoPlayer
-  init(player:) 

Initializer

# init(player:)

Creates a video-player user interface for the player object.

AVKitSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
init(player: AVPlayer?)
```

Available when `VideoOverlay` is `EmptyView`.

## Parameters 

`player`  

The player that plays the audiovisual content.

## See Also

### Creating a Video Player

init(player: AVPlayer?, videoOverlay: () -> VideoOverlay)

Creates a video-player user interface for the player object.

