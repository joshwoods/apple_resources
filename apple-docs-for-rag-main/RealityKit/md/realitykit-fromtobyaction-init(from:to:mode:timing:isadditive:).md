

- RealityKit
- FromToByAction
-  init(from:to:mode:timing:isAdditive:) 

Initializer

# init(from:to:mode:timing:isAdditive:)

Creates a new action that interpolates towards a specified final transform.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    from: Value? = nil,
    to: Value,
    mode: FromToByAction.TransformMode = .default,
    timing: AnimationTimingFunction = .linear,
    isAdditive: Bool = false
)
```

Available when `Value` is `Transform`.

## Parameters 

`from`  

Transform set at the start of the animation, or `nil` to use the default source.

`to`  

Transform set at the end of the animation.

`mode`  

Determines what space the transforms are relative to.

`timing`  

Controls the progress of the animation.

`isAdditive`  

Specifies whether you can additively blend the output from the action’s animation.

## Discussion

`defaultSource` → `to` or `defaultSource` → `to`

