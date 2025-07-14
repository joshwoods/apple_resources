

- Accelerate
-  BNNSGraphContextMake(\_:) 

Function

# BNNSGraphContextMake(\_:)

Returns an allocated and initialized graph context from the specified graph.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextMake(_ graph: bnns_graph_t) -> bnns_graph_context_t
```

## Parameters 

`graph`  

The compiled graph object.

## Return Value

A compiled graph context object. If the operation fails, the graph object’s data property is `nil`.

## Discussion

To prevent memory leaks, call BNNSGraphContextDestroy(_:) when you’re finished using the graph context.

## See Also

### Creating and destroying a context

struct bnns_graph_context_t

An object that wraps a compiled graph object.

func BNNSGraphContextMakeStreaming(bnns_graph_t, UnsafePointer&lt;CChar>?, Int, UnsafePointer&lt;BNNSTensor>?) -> bnns_graph_context_t

Returns an allocated and initialized graph context with streaming support from the specified graph.

func BNNSGraphContextDestroy(bnns_graph_context_t)

Destroys the specified graph context.

