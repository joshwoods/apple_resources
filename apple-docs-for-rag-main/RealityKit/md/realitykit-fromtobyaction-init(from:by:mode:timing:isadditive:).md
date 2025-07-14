

- RealityKit
- FromToByAction
-  init(from:by:mode:timing:isAdditive:) 

Initializer

# init(from:by:mode:timing:isAdditive:)

Creates a new action that interpolates from a specified starting transform towards a specified transform, which is relative to the start. Alternatively, interpolates towards the default source if `by` is not supplied.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    from: Value,
    by: Value? = nil,
    mode: FromToByAction.TransformMode = .default,
    timing: AnimationTimingFunction = .linear,
    isAdditive: Bool = false
)
```

Available when `Value` is `Transform`.

## Parameters 

`from`  

Transform set at the start of the animation.

`by`  

Transform which is used to increment the starting transform. Used to determine the final transform we animate towards. Set this to `nil` to animate towards the defaultSource transform.

`mode`  

Determines what space the transforms are relative to.

`timing`  

Controls the progress of the animation.

`isAdditive`  

Specifies whether you can additively blend the output from the action’s animation.

## Discussion

`from` → `from + by` or `from` → `defaultSource`

