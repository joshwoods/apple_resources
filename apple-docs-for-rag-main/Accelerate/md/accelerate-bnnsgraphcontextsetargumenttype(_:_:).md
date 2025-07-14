

- Accelerate
-  BNNSGraphContextSetArgumentType(\_:\_:) 

Function

# BNNSGraphContextSetArgumentType(\_:\_:)

Specifies the argument type for a graph context.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextSetArgumentType(
    _ context: bnns_graph_context_t,
    _ argument_type: BNNSGraphArgumentType
) -> Int32
```

## Parameters 

`context`  

The graph context.

`argument_type`  

A constant that specifies the argument type.

## Return Value

`0` on success, nonzero on failure.

## Discussion

Some arguments require dynamic strides. In this case, set the graph context’s argument type to BNNSGraphArgumentTypeTensor and pass the arguments to BNNSGraphContextExecute(_:_:_:_:_:_:) as BNNSTensor structures.

The default argument type for a graph context is BNNSGraphArgumentTypePointer.

## See Also

### Specifying and querying a context’s properties

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

func BNNSGraphContextGetWorkspaceSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?) -> Int

Returns the minimum size, in bytes, of the workspace that graph context execution requires.

