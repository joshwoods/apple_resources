

- RealityKit
- Entity
-  move(to:relativeTo:duration:timingFunction:) 

Instance Method

# move(to:relativeTo:duration:timingFunction:)

Moves an entity over a period of time to a new location given by a 4x4 matrix.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@discardableResult @MainActor @preconcurrency
func move(
    to target: float4x4,
    relativeTo referenceEntity: Entity?,
    duration: TimeInterval,
    timingFunction: AnimationTimingFunction = .default
) -> AnimationPlaybackController
```

## Parameters 

`target`  

A 4x4 matrix that indicates the new location.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

`duration`  

The time in seconds over which the move should occur.

`timingFunction`  

A timing function that controls the progress of the animation.

## Return Value

An AnimationPlaybackController instance that you use to control the animation playback.

