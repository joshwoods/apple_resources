

- RealityKit
- AnimationPlaybackController
-  isComplete 

Instance Property

# isComplete

A Boolean that indicates whether the animation has finished running.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var isComplete: Bool { get }
```

## Discussion

After an animation completes, the playback controller becomes invalid. To play the animation again, create a new controller with the same resource.

## See Also

### Managing completion

var isPaused: Bool

A Boolean that indicates whether the animation is paused.

