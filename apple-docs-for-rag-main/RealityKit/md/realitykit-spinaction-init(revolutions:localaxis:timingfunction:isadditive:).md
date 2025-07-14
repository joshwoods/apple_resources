

- RealityKit
- SpinAction
-  init(revolutions:localAxis:timingFunction:isAdditive:) 

Initializer

# init(revolutions:localAxis:timingFunction:isAdditive:)

Creates a new spin action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    revolutions: Float,
    localAxis: SIMD3 = [0, 1, 0],
    timingFunction: AnimationTimingFunction = .default,
    isAdditive: Bool = false
)
```

## Parameters 

`revolutions`  

The number of rotations to complete before stopping.

`localAxis`  

A vector that describes the axis of rotation (in local space).

`timingFunction`  

A timing function that controls the progress of the animation.

`isAdditive`  

A Boolean value that indicates whether the animation system additively blends the action’s output with the base value.

