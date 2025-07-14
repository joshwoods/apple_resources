

- RealityKit
- AnimationPlaybackController
-  isStopped 

Instance Property

# isStopped

A Boolean value that indicates whether the animation stopped.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
var isStopped: Bool { get }
```

## Discussion

This function returns `true` for stopped animations.

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

var isValid: Bool

A Boolean value that indicates whether the animation controller is functional.

var blendFactor: Float

The level of influence the controller gives to its animation.

