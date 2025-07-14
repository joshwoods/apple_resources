

- RealityKit
- AnimationPlaybackController
-  isValid 

Instance Property

# isValid

A Boolean value that indicates whether the animation controller is functional.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
var isValid: Bool { get }
```

## Discussion

This function returns `false` for stopped animations.

## See Also

### Inspecting and controlling playback

func pause()

Pauses the animation.

func resume()

Resumes a paused animation.

func stop()

Stops an animation.

var isPlaying: Bool

A Boolean value that indicates whether the animation plays.

var isStopped: Bool

A Boolean value that indicates whether the animation stopped.

var blendFactor: Float

The level of influence the controller gives to its animation.

