

- Accelerate
- bnns_graph_t
-  init(data:size:) 

Initializer

# init(data:size:)

Creates a graph structure from the specified opaque graph object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    data: UnsafeMutableRawPointer?,
    size: Int
)
```

## Parameters 

`data`  

A pointer to opaque graph object.

`size`  

The size, in bytes, of the opaque graph object.

## See Also

### Initializing a graph

init()

Creates an empty graph structure.

