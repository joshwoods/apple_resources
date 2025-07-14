

- Accelerate
-  bnns_graph_shape_t 

Structure

# bnns_graph_shape_t

The specification of the shape of an argument.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct bnns_graph_shape_t
```

## Overview

Use a bnns_graph_shape_t structure to pass the rank and dimensions of tensors to the BNNSGraphContextSetDynamicShapes(_:_:_:_:) function.

## Topics

### Initializing a graph shape

init()

Creates an empty shape structure.

init(rank: Int, shape: UnsafeMutablePointer&lt;UInt64>?)

Creates a shape structure with the specified rank and dimensions.

### Specifying a shape’s properties

var rank: Int

The rank of the shape.

var shape: UnsafeMutablePointer&lt;UInt64>?

An array of unsigned-integer elements that specify the size of the shape.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Specifying and querying a context’s properties

func BNNSGraphContextSetArgumentType(bnns_graph_context_t, BNNSGraphArgumentType) -> Int32

Specifies the argument type for a graph context.

struct BNNSGraphArgumentType

Constants that specify the argument type for a graph context.

func BNNSGraphContextSetDynamicShapes(bnns_graph_context_t, UnsafePointer&lt;CChar>?, Int, UnsafeMutablePointer&lt;bnns_graph_shape_t>) -> Int32

Specifies the dynamic shapes for a graph and, if possible, infers, the output shapes.

func BNNSGraphContextSetBatchSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?, UInt64) -> Int32

Sets the batch size for a graph.

func BNNSGraphContextEnableNanAndInfChecks(bnns_graph_context_t, Bool)

Specifies that the context checks intermediate tensors for NaNs and infinities.

func BNNSGraphContextGetWorkspaceSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?) -> Int

Returns the minimum size, in bytes, of the workspace that graph context execution requires.

