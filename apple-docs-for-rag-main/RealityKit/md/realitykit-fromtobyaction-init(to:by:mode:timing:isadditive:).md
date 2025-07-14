

- RealityKit
- FromToByAction
-  init(to:by:mode:timing:isAdditive:) 

Initializer

# init(to:by:mode:timing:isAdditive:)

Creates a action to animate towards a final value. The starting value is determined by adding the inverse of `by` to the specified final value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    to: Value,
    by: Value,
    mode: FromToByAction.TransformMode = .default,
    timing: AnimationTimingFunction = .linear,
    isAdditive: Bool = false
)
```

Available when `Value` is `Transform`.

## Parameters 

`to`  

Value set at the end of the animation.

`by`  

Value used to determine the starting value, relative to the end value.

`mode`  

Determines what space the transforms are relative to.

`timing`  

Controls the progress of the animation.

`isAdditive`  

Specifies whether you can additively blend the output from the action’s animation.

## Discussion

`to - by` → `to`

