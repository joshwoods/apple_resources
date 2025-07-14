

- Accelerate
-  BNNSGraphContextGetWorkspaceSize(\_:\_:) 

Function

# BNNSGraphContextGetWorkspaceSize(\_:\_:)

Returns the minimum size, in bytes, of the workspace that graph context execution requires.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextGetWorkspaceSize(
    _ context: bnns_graph_context_t,
    _ function: UnsafePointer?
) -> Int
```

## Parameters 

`context`  

The graph context.

`function`  

The function. Specify as `nil` if the graph only contains one function.

## Return Value

The minimum size, in bytes, for the workspace, or `SIZE_T_MAX` if the query fails.

## Discussion

Call this function to obtain the minimum size of the workspace that the BNNSGraphContextExecute function requires. If you call either BNNSGraphContextSetBatchSize(_:_:_:) or BNNSGraphContextSetDynamicShapes(_:_:_:_:), call this function afterwards to obtain the new workspace size.

Note that the workspace size may not be proportional with the dynamic size. That is, smaller input and output tensors may require a larger workspace.

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

func BNNSGraphContextSetBatchSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?, UInt64) -> Int32

Sets the batch size for a graph.

func BNNSGraphContextEnableNanAndInfChecks(bnns_graph_context_t, Bool)

Specifies that the context checks intermediate tensors for NaNs and infinities.

