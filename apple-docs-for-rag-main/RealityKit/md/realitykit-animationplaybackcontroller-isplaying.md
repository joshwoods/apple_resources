

- RealityKit
- AnimationPlaybackController
-  isPlaying 

Instance Property

# isPlaying

A Boolean value that indicates whether the animation plays.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
var isPlaying: Bool { get }
```

## See Also

### Inspecting and controlling playback

func pause()

Pauses the animation.

func resume()

Resumes a paused animation.

func stop()

Stops an animation.

var isStopped: Bool

A Boolean value that indicates whether the animation stopped.

var isValid: Bool

A Boolean value that indicates whether the animation controller is functional.

var blendFactor: Float

The level of influence the controller gives to its animation.

