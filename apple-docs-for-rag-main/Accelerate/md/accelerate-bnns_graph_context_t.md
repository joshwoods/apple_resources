

- Accelerate
-  bnns_graph_context_t 

Structure

# bnns_graph_context_t

An object that wraps a compiled graph object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct bnns_graph_context_t
```

## Overview

The bnns_graph_context_t object wraps a bnns_graph_t instance and adds mutable data storage. BNNS requires mutability to support dynamic shapes and other execution objects.

You must ensure that the underlying bnns_graph_t instance remains valid throughout the lifetime of the context.

## Topics

### Initializing a context

init()

Creates an empty graph context structure.

init(data: UnsafeMutableRawPointer?, size: Int)

Creates a graph context structure from the specified opaque graph context object.

### Specifying a context’s properties

var data: UnsafeMutableRawPointer?

A pointer to the opaque graph context object.

var size: Int

The size, in bytes, of the opaque graph context object.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Creating and destroying a context

func BNNSGraphContextMake(bnns_graph_t) -> bnns_graph_context_t

Returns an allocated and initialized graph context from the specified graph.

func BNNSGraphContextMakeStreaming(bnns_graph_t, UnsafePointer&lt;CChar>?, Int, UnsafePointer&lt;BNNSTensor>?) -> bnns_graph_context_t

Returns an allocated and initialized graph context with streaming support from the specified graph.

func BNNSGraphContextDestroy(bnns_graph_context_t)

Destroys the specified graph context.

