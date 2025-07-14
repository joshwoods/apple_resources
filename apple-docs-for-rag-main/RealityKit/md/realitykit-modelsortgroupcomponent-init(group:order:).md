

- RealityKit
- ModelSortGroupComponent
-  init(group:order:) 

Initializer

# init(group:order:)

Creates a model sort group component.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(
    group: ModelSortGroup,
    order: Int32
)
```

## Parameters 

`group`  

A group the component’s entity belongs to.

`order`  

An integer value in the range `(Int32.min, Int32.max)` that represents when the renderer draws the model relative to other the models in its group.

## Discussion

Warning

Don’t pass `Int32.max` or `Int32.min` to the `order` parameter because the framework reserves these as sentinel values, and using them may trigger erratic behavior.

