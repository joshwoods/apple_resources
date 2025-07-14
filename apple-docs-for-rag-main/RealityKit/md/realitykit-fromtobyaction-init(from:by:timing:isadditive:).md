

- RealityKit
- FromToByAction
-  init(from:by:timing:isAdditive:) 

Initializer

# init(from:by:timing:isAdditive:)

Creates a new action that interpolates towards a specified value, which is relative to the starting value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    from: Value? = nil,
    by: Value,
    timing: AnimationTimingFunction = .linear,
    isAdditive: Bool = false
)
```

## Parameters 

`from`  

Value set at the start of the animation, or `nil` to use the default source.

`by`  

Value relative to the initial value to determine the final value.

`timing`  

Controls the progress of the animation.

`isAdditive`  

Specifies whether you can additively blend the output from the action’s animation.

## Discussion

`from` → `from + by` or `defaultSource` → `defaultSource + by`

