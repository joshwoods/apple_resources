

- RealityKit
- Entity
-  availableAnimations 

Instance Property

# availableAnimations

The list of animations associated with the entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var availableAnimations: [AnimationResource] { get }
```

## Discussion

When you import an entity from a file, for example by using the load(named:in:) method, the entity might contain associated animations. Any that RealityKit supports appear in the availableAnimations array.

To play a particular animation resource from the list, call the playAnimation(_:transitionDuration:startsPaused:) method. Alternatively, to play all animations with a given name, call the `playAnimation(named:transitionDuration:startsPaused:)` method instead.

## See Also

### Animating an entity

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

var parameters: Entity.ParameterSet

Represents a reference to the parameters for a particular entity.

struct ParameterSet

Represents a reference to the parameters for a particular entity.

func playAnimation(named: String, transitionDuration: TimeInterval, startsPaused: Bool, recursive: Bool) -> AnimationPlaybackController

Plays all the animations with the given name on the entity.

Deprecated

var bindableValues: BindableValuesReference

subscript(BindTarget.EntityPath) -> Entity?

Resolves the entity from the given entity path.

