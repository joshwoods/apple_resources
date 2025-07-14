

- RealityKit
- FromToByAction
-  init(by:timing:isAdditive:) 

Initializer

# init(by:timing:isAdditive:)

Creates a new action to animate from the deaultSource by a transform relative to the starting transform.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    by: Value,
    timing: AnimationTimingFunction = .linear,
    isAdditive: Bool = false
)
```

Available when `Value` is `Transform`.

## Parameters 

`by`  

Transform which is used to increment the starting transform. Used to determine the final transform we animate towards.

`timing`  

Controls the progress of the animation.

`isAdditive`  

Specifies whether you can additively blend the output from the action’s animation.

## Discussion

`defaultSource` → `defaultSource + by`

