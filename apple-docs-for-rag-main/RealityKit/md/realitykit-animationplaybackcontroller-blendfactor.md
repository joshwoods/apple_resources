

- RealityKit
- AnimationPlaybackController
-  blendFactor 

Instance Property

# blendFactor

The level of influence the controller gives to its animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
var blendFactor: Float { get set }
```

## Discussion

You can run multiple animations on the same property, for example, walking and jumping animations that affect the same joint transforms. When multiple animations adjust the same property at runtime, the framework applies this blend factor on the animations’ respective controllers to calculate a middle ground value that displays at runtime.

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

var isValid: Bool

A Boolean value that indicates whether the animation controller is functional.

