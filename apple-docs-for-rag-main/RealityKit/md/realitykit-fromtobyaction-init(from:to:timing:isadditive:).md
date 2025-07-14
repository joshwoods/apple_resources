

- RealityKit
- FromToByAction
-  init(from:to:timing:isAdditive:) 

Initializer

# init(from:to:timing:isAdditive:)

Creates a new action that interpolates towards a specified final value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    from: Value? = nil,
    to: Value,
    timing: AnimationTimingFunction = .linear,
    isAdditive: Bool = false
)
```

## Parameters 

`from`  

Value set at the start of the animation, or `nil` to use the default source.

`to`  

Value set at the end of the animation.

`timing`  

Controls the progress of the animation.

`isAdditive`  

A Boolean value that indicates whether the animation system additively blends the action’s output with the base value.

## Discussion

`from` → `to` or `defaultSource` → `to`

