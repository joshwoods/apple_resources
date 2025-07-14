

- AVKit
- VideoPlayer
-  init(player:videoOverlay:) 

Initializer

# init(player:videoOverlay:)

Creates a video-player user interface for the player object.

AVKitSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
init(
    player: AVPlayer?,
    @ViewBuilder videoOverlay: () -> VideoOverlay
)
```

## Parameters 

`player`  

The player that plays the audiovisual content.

`videoOverlay`  

A closure that returns a `VideoOverlay` view to present over the player’s video content. This view is fully interactive, but is placed below the system-provided playback controls, and only receives unhandled events.

## See Also

### Creating a Video Player

init(player: AVPlayer?)

Creates a video-player user interface for the player object.

