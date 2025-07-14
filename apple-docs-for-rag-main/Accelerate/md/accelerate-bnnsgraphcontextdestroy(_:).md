

- Accelerate
-  BNNSGraphContextDestroy(\_:) 

Function

# BNNSGraphContextDestroy(\_:)

Destroys the specified graph context.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextDestroy(_ context: bnns_graph_context_t)
```

## Parameters 

`context`  

The graph context.

## See Also

### Creating and destroying a context

struct bnns_graph_context_t

An object that wraps a compiled graph object.

func BNNSGraphContextMake(bnns_graph_t) -> bnns_graph_context_t

Returns an allocated and initialized graph context from the specified graph.

func BNNSGraphContextMakeStreaming(bnns_graph_t, UnsafePointer&lt;CChar>?, Int, UnsafePointer&lt;BNNSTensor>?) -> bnns_graph_context_t

Returns an allocated and initialized graph context with streaming support from the specified graph.

