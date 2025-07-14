

- RealityKit
- Entity
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Resolves the entity from the given entity path.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
subscript(entityPath: BindTarget.EntityPath) -> Entity? { get }
```

## Parameters 

`entityPath`  

The entity path to resolve.

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

var parameters: Entity.ParameterSet

Represents a reference to the parameters for a particular entity.

struct ParameterSet

Represents a reference to the parameters for a particular entity.

func playAnimation(named: String, transitionDuration: TimeInterval, startsPaused: Bool, recursive: Bool) -> AnimationPlaybackController

Plays all the animations with the given name on the entity.

Deprecated

var bindableValues: BindableValuesReference

