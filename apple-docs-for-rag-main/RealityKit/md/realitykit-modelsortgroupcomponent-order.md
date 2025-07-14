

- RealityKit
- ModelSortGroupComponent
-  order 

Instance Property

# order

An integer value that represents when the renderer draws the model relative to other the models in its group.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var order: Int32 { get set }
```

## Discussion

The renderer draws models in ascending order, starting with the components with the smallest value. You can tell the renderer that it only needs to order entities by their depths by setting the component’s order property to the sam value for those entities.

Warning

Don’t set `order` to `Int32.max` or `Int32.min` because the framework reserves these as sentinel values, and assigning their values may trigger erratic behavior.

