

- Accelerate
-  bnns_graph_t 

Structure

# bnns_graph_t

The compiled graph object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct bnns_graph_t
```

## Topics

### Initializing a graph

init()

Creates an empty graph structure.

init(data: UnsafeMutableRawPointer?, size: Int)

Creates a graph structure from the specified opaque graph object.

### Instance properties

var data: UnsafeMutableRawPointer?

A pointer to opaque graph object.

var size: Int

The size, in bytes, of the opaque graph object.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Compiling a graph object

func BNNSGraphCompileFromFile(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>?, bnns_graph_compile_options_t) -> bnns_graph_t

Compiles a source mlmodelc file to a graph object.

