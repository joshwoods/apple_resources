

- Accelerate
- bnns_graph_compile_options_t
-  init(data:size:) 

Initializer

# init(data:size:)

Creates a compilation options structure from the specified opaque compilation options object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    data: UnsafeMutableRawPointer?,
    size: Int
)
```

## Parameters 

`data`  

A pointer to opaque compilation options object.

`size`  

The size, in bytes, of the opaque compilation options object.

## See Also

### Initializing an options structure

init()

Creates an empty compilation options structure.

