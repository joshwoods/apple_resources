

- RealityKit
- Entity
-  parameters 

Instance Property

# parameters

Represents a reference to the parameters for a particular entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
var parameters: Entity.ParameterSet { get set }
```

## See Also

### Animating an entity

var availableAnimations: [AnimationResource]

The list of animations associated with the entity.

func playAnimation(AnimationResource, transitionDuration: TimeInterval, blendLayerOffset: Int, separateAnimatedValue: Bool, startsPaused: Bool, clock: CMClockOrTimebase?) -> AnimationPlaybackController

Plays an animation with the specified options.

func playAnimation(AnimationResource, transitionDuration: TimeInterval, blendLayerOffset: Int, separateAnimatedValue: Bool, startsPaused: Bool, clock: CMClockOrTimebase?, handoffType: AnimationHandoffType) -> AnimationPlaybackController

Plays an animation with the specified options.

func playAnimation(AnimationResource, transitionDuration: TimeInterval, startsPaused: Bool) -> AnimationPlaybackController

Plays the given animation on the entity.

func stopAllAnimations(recursive: Bool)

Stops all playing of animations on this entity.

var defaultAnimationClock: CMClockOrTimebase

Returns the default animation clock for this entity.

struct ParameterSet

Represents a reference to the parameters for a particular entity.

func playAnimation(named: String, transitionDuration: TimeInterval, startsPaused: Bool, recursive: Bool) -> AnimationPlaybackController

Plays all the animations with the given name on the entity.

Deprecated

var bindableValues: BindableValuesReference

subscript(BindTarget.EntityPath) -> Entity?

Resolves the entity from the given entity path.

