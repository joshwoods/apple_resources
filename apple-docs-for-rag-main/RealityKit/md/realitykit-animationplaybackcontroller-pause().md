

- RealityKit
- AnimationPlaybackController
-  pause() 

Instance Method

# pause()

Pauses the animation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func pause()
```

## Discussion

Resume a paused animation by calling the resume() method.

This method has no effect if the animation is already paused or complete.

## See Also

### Inspecting and controlling playback

func resume()

Resumes a paused animation.

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

