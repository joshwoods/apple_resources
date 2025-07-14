

- Accelerate
- bnns_graph_context_t
-  init(data:size:) 

Initializer

# init(data:size:)

Creates a graph context structure from the specified opaque graph context object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    data: UnsafeMutableRawPointer?,
    size: Int
)
```

## Parameters 

`data`  

A pointer to opaque graph context object.

`size`  

The size, in bytes, of the opaque graph context object.

## See Also

### Initializing a context

init()

Creates an empty graph context structure.

