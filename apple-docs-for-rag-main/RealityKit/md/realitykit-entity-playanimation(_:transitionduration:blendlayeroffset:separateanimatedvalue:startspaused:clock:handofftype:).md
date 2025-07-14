

- RealityKit
- Entity
-  playAnimation(\_:transitionDuration:blendLayerOffset:separateAnimatedValue:startsPaused:clock:handoffType:) 

Instance Method

# playAnimation(\_:transitionDuration:blendLayerOffset:separateAnimatedValue:startsPaused:clock:handoffType:)

Plays an animation with the specified options.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@discardableResult @MainActor @preconcurrency
func playAnimation(
    _ animation: AnimationResource,
    transitionDuration: TimeInterval = 0,
    blendLayerOffset: Int = 0,
    separateAnimatedValue: Bool = false,
    startsPaused: Bool = false,
    clock: CMClockOrTimebase? = nil,
    handoffType: AnimationHandoffType = .default
) -> AnimationPlaybackController
```

## Parameters 

`animation`  

The animation to play.

`transitionDuration`  

The duration in seconds over which the animation fades in or cross-fades.

`blendLayerOffset`  

An integer that specifies the order in which to apply animations when more than one animation is playing.

`separateAnimatedValue`  

When set to false, this value indicates that the animation will write directly to the entity’s base value. When set to true, this value indicates that the animation will write to an interim value for the duration of the animation. If this value is set to true then when the animation completes, the entity’s value will be reset to the base value.

`startsPaused`  

A Boolean that pauses the progress of an animation when set to `true`.

`clock`  

An optional clock to drive the animation with a custom timescale.

`handoffType`  

Type of handoff behavior between a currently-playing animation and the new animation. Defaults to `.snapshotAndReplace(applyToAllLayers: true)`.

## Discussion

Call this method to play an animation and configure playback options. RealityKit supports blending up to two different animations at the same time. When RealityKit applies multiple animations to an entity, the order in which it applies the animations affects the final animation. Use the `blendLayerOffset` parameter to specify the order of animations when playing multiple animations at the same time.

## See Also

### Animating an entity

var availableAnimations: [AnimationResource]

The list of animations associated with the entity.

func playAnimation(AnimationResource, transitionDuration: TimeInterval, blendLayerOffset: Int, separateAnimatedValue: Bool, startsPaused: Bool, clock: CMClockOrTimebase?) -> AnimationPlaybackController

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

