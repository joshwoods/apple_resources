

- RealityKit
- PlayAnimationAction
-  init(animationName:targetEntity:transitionDuration:blendLayer:separateAnimatedValue:useParentedControllers:handoffType:) 

Initializer

# init(animationName:targetEntity:transitionDuration:blendLayer:separateAnimatedValue:useParentedControllers:handoffType:)

Creates a new play animation action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    animationName: String,
    targetEntity: ActionEntityResolution = .sourceEntity,
    transitionDuration: TimeInterval = 0.0,
    blendLayer: Int = 0,
    separateAnimatedValue: Bool = true,
    useParentedControllers: Bool = false,
    handoffType: AnimationHandoffType = .compose
)
```

## Parameters 

`animationName`  

The name of the animation resource within the target entity animation library component to start playing.

`targetEntity`  

The entity to play the animation.

`transitionDuration`  

The duration in seconds over which the animation fades in or cross-fades.

`blendLayer`  

An integer that specifies the order in which to apply animations when more than one animation is playing.

`separateAnimatedValue`  

When set to false, this value indicates that the animation will write directly to the entity’s base value. When set to true, this value indicates that the animation will write to an interim value for the duration of the animation. If this value is set to true then when the animation completes, the entity’s value will be reset to the base value.

`useParentedControllers`  

Whether to parent the new animation’s controller to the controller managing this action.

`handoffType`  

Type of handoff behavior between a currently-playing animation and the new animation.

