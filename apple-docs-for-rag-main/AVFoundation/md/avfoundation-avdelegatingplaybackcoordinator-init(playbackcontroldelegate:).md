

- AVFoundation
- AVDelegatingPlaybackCoordinator
-  init(playbackControlDelegate:) 

Initializer

# init(playbackControlDelegate:)

Creates a playback coordinator for a custom playback object.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
init(playbackControlDelegate: any AVPlaybackCoordinatorPlaybackControlDelegate)
```

## Parameters 

`playbackControlDelegate`  

The playback control delegate for the playback coordinator.

## Discussion

If your app doesn’t use AVPlayer for playback, create an instance of this class to coordinate playback of your customer player.

## See Also

### Creating a Coordinator

protocol AVPlaybackCoordinatorPlaybackControlDelegate

A protocol that defines the method to implement to respond to playback commands from the playback coordinator.

