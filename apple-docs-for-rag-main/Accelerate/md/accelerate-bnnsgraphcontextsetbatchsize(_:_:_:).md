

- Accelerate
-  BNNSGraphContextSetBatchSize(\_:\_:\_:) 

Function

# BNNSGraphContextSetBatchSize(\_:\_:\_:)

Sets the batch size for a graph.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextSetBatchSize(
    _ context: bnns_graph_context_t,
    _ function: UnsafePointer?,
    _ batch_size: UInt64
) -> Int32
```

## Parameters 

`context`  

The graph context.

`function`  

The function. Specify as `nil` if the graph only contains one function.

`batch_size`  

The batch size.

## Return Value

`0` on success, nonzero on failure.

## Discussion

This function provides a special case of BNNSGraphContextSetDynamicShapes(_:_:_:_:) where the only dynamic size is the first index of the tensors and that size is equal for all tensors. This function provides a simpler API because you only need to pass the common first dimension as the `batch_size` parameter.

If your graph contains other dynamic strides, use BNNSGraphContextSetDynamicShapes(_:_:_:_:) instead. This function doesn’t set dynamic strides.

Don’t call this function while existing calls to BNNSGraphContextExecute(_:_:_:_:_:_:) are running.

## See Also

### Specifying and querying a context’s properties

func BNNSGraphContextSetArgumentType(bnns_graph_context_t, BNNSGraphArgumentType) -> Int32

Specifies the argument type for a graph context.

struct BNNSGraphArgumentType

Constants that specify the argument type for a graph context.

func BNNSGraphContextSetDynamicShapes(bnns_graph_context_t, UnsafePointer&lt;CChar>?, Int, UnsafeMutablePointer&lt;bnns_graph_shape_t>) -> Int32

Specifies the dynamic shapes for a graph and, if possible, infers, the output shapes.

struct bnns_graph_shape_t

The specification of the shape of an argument.

func BNNSGraphContextEnableNanAndInfChecks(bnns_graph_context_t, Bool)

Specifies that the context checks intermediate tensors for NaNs and infinities.

func BNNSGraphContextGetWorkspaceSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?) -> Int

Returns the minimum size, in bytes, of the workspace that graph context execution requires.

