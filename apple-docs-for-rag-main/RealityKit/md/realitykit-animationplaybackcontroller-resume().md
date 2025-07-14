

- RealityKit
- AnimationPlaybackController
-  resume() 

Instance Method

# resume()

Resumes a paused animation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func resume()
```

## Discussion

Call this method to resume an animation that you paused with the pause() method. You can’t resume an animation that has finished naturally, or that you stopped by calling the stop() method.

This method has no effect on an animation that isn’t paused.

## See Also

### Inspecting and controlling playback

func pause()

Pauses the animation.

func stop()

Stops an animation.

var isPlaying: Bool

A Boolean value that indicates whether the animation plays.

var isStopped: Bool

A Boolean value that indicates whether the animation stopped.

var isValid: Bool

A Boolean value that indicates whether the animation controller is functional.

var blendFactor: Float

The level of influence the controller gives to its animation.

