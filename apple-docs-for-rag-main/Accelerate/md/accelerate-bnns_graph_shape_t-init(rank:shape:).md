

- Accelerate
- bnns_graph_shape_t
-  init(rank:shape:) 

Initializer

# init(rank:shape:)

Creates a shape structure with the specified rank and dimensions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    rank: Int,
    shape: UnsafeMutablePointer?
)
```

## Parameters 

`rank`  

The rank of the tensor and number of elements in array shape.

`shape`  

Array with a count of rank that contains the sizes of each dimension.

## See Also

### Initializing a graph shape

init()

Creates an empty shape structure.

