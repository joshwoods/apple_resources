

- RealityKit
- Entity
-  playAnimation(named:transitionDuration:startsPaused:recursive:) Deprecated

Instance Method

# playAnimation(named:transitionDuration:startsPaused:recursive:)

Plays all the animations with the given name on the entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@discardableResult @MainActor @preconcurrency
func playAnimation(
    named animationName: String,
    transitionDuration: TimeInterval = 0,
    startsPaused: Bool = false,
    recursive: Bool = true
) -> AnimationPlaybackController
```

Deprecated

Use playAnimation functions that utilize an AnimationResource instead of a name.

## Parameters 

`animationName`  

The name of the animation.

`transitionDuration`  

The duration in seconds over which the animation fades in or cross-fades.

`startsPaused`  

A Boolean that you set to `true` to return from the call with the animations paused. Set to `false` to start the animations right away.

`recursive`  

Indicates whether to also play animations on all descendants of the entity.

## Return Value

An animation playback controller that you can use to start and stop the animations.

## Discussion

The method plays all the animations in the availableAnimations property with a matching name. If there are none, the method returns a controller showing a stopped animation.

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

var bindableValues: BindableValuesReference

subscript(BindTarget.EntityPath) -> Entity?

Resolves the entity from the given entity path.

