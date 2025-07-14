

- Accelerate
-  BNNSGraphContextEnableNanAndInfChecks(\_:\_:) 

Function

# BNNSGraphContextEnableNanAndInfChecks(\_:\_:)

Specifies that the context checks intermediate tensors for NaNs and infinities.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextEnableNanAndInfChecks(
    _ context: bnns_graph_context_t,
    _ enable_check_for_nans_inf: Bool
)
```

## Parameters 

`context`  

The graph context.

`enable_check_for_nans_inf`  

If `true`, specifies that the context checks intermediate tensors for NaNs and infinities.

## Discussion

Don’t enable this option for production code.

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

func BNNSGraphContextGetWorkspaceSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?) -> Int

Returns the minimum size, in bytes, of the workspace that graph context execution requires.

