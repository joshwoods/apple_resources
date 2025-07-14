

- RealityKit
- AnimationPlaybackController
-  stop(blendOutDuration:) 

Instance Method

# stop(blendOutDuration:)

Stops an animation with a fade-out time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func stop(blendOutDuration: TimeInterval)
```

## Parameters 

`blendOutDuration`  

Time (in seconds) to fade out the animation before it stops.

## Discussion

This method has no effect if the animation is complete. After you stop the animation, the playback controller becomes invalid. Create a new one with the same resource to play the animation again.

