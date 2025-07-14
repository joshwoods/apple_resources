

- RealityKit
- Entity
-  playAnimation(\_:transitionDuration:startsPaused:) 

Instance Method

# playAnimation(\_:transitionDuration:startsPaused:)

Plays the given animation on the entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@discardableResult @MainActor @preconcurrency
func playAnimation(
    _ animation: AnimationResource,
    transitionDuration: TimeInterval,
    startsPaused: Bool
) -> AnimationPlaybackController
```

## Parameters 

`animation`  

The animation to play.

`transitionDuration`  

The duration in seconds over which the animation fades in or cross-fades.

`startsPaused`  

A Boolean that you set to `true` to return from the call with the animation paused. Set to `false` to start the animation right away.

## Return Value

An animation playback controller that you can use to start and stop the animation.

## See Also

### Animating an entity

var availableAnimations: [AnimationResource]

The list of animations associated with the entity.

func playAnimation(AnimationResource, transitionDuration: TimeInterval, blendLayerOffset: Int, separateAnimatedValue: Bool, startsPaused: Bool, clock: CMClockOrTimebase?) -> AnimationPlaybackController

Plays an animation with the specified options.

func playAnimation(AnimationResource, transitionDuration: TimeInterval, blendLayerOffset: Int, separateAnimatedValue: Bool, startsPaused: Bool, clock: CMClockOrTimebase?, handoffType: AnimationHandoffType) -> AnimationPlaybackController

Plays an animation with the specified options.

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

