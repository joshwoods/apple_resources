

- RealityKit
- AnimationResource
-  name 

Instance Property

# name

The name of the animation resource.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
final let name: String?
```

## Discussion

You can get an AnimationPlaybackController instance ready to play a particular resource that you reference by its name using the `playAnimation(named:transitionDuration:startsPaused:)` method.

## See Also

### Inspecting animation information

var definition: any AnimationDefinition

The timeframe, target object, and visual semantics of the animation.

struct AnimationFillMode

Options that determine which animation frames display outside of the normal duration.

