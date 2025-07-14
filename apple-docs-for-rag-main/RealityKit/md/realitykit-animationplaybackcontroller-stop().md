

- RealityKit
- AnimationPlaybackController
-  stop() 

Instance Method

# stop()

Stops an animation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func stop()
```

## Discussion

This method has no effect if the animation is complete. After you stop the animation, the playback controller becomes invalid. Create a new one with the same resource to play the animation again.

## See Also

### Inspecting and controlling playback

func pause()

Pauses the animation.

func resume()

Resumes a paused animation.

var isPlaying: Bool

A Boolean value that indicates whether the animation plays.

var isStopped: Bool

A Boolean value that indicates whether the animation stopped.

var isValid: Bool

A Boolean value that indicates whether the animation controller is functional.

var blendFactor: Float

The level of influence the controller gives to its animation.

