

- RealityKit
- Entity
-  move(to:relativeTo:duration:timingFunction:) 

Instance Method

# move(to:relativeTo:duration:timingFunction:)

Moves an entity over a period of time to a new location given by a transform.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@discardableResult @MainActor @preconcurrency
func move(
    to target: Transform,
    relativeTo referenceEntity: Entity?,
    duration: TimeInterval,
    timingFunction: AnimationTimingFunction = .default
) -> AnimationPlaybackController
```

## Parameters 

`target`  

A Transform instance that indicates the new location.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

`duration`  

The time in seconds over which the move should occur.

`timingFunction`  

A timing function that controls the progress of the animation.

## Return Value

An AnimationPlaybackController instance that you use to control the animation playback.

## Discussion

Animating the scale of an entity to 0 will cause a subsequent inverse of the entity’s transform to return NaN values. Developers may consider animating the scale of an entity to a small non-zero value. When the move completes, the entity can then be hidden or removed if applicable to the use case.

