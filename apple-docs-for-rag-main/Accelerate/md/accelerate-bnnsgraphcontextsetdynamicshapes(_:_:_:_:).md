

- Accelerate
-  BNNSGraphContextSetDynamicShapes(\_:\_:\_:\_:) 

Function

# BNNSGraphContextSetDynamicShapes(\_:\_:\_:\_:)

Specifies the dynamic shapes for a graph and, if possible, infers, the output shapes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextSetDynamicShapes(
    _ context: bnns_graph_context_t,
    _ function: UnsafePointer?,
    _ shapes_count: Int,
    _ shapes: UnsafeMutablePointer
) -> Int32
```

## Parameters 

`context`  

The graph context.

`function`  

The function. Specify as `nil` if the graph only contains one function.

`shapes_count`  

The number of elements in the `shapes` array.

`shapes`  

An array of input and output shapes in the same order as you pass to BNNSGraphContextExecute(_:_:_:_:_:_:).

On input, this function reads input shapes with a nonzero rank, and uses the constant or default value from the source model for input shapes with a zero rank. The function generates an error for shapes with a nonzero value that doesn’t match the source model.

On output, the function sets output shapes with a nonzero rank to the upper bounds of the expected output shape. If the function can’t deduce the output shape because it depends on the input data values, the value of `shapes[idx].size[d]` is zero.

## Return Value

\- `0` on success if all tensor shapes were exactly determined. That is, the workspace size is exact.

## Discussion

- `1` on success if one or more tensor shapes are merely bounds, but no tensor is unbounded. That is, the workspace size is bounded.

- `2` on success if one or more tensor shapes are unbounded and BNNS will allocate workspace memory during execution.

- A negative value indicates an error.

## Discussion

Don’t call this function while existing calls to BNNSGraphContextExecute(_:_:_:_:_:_:) are running.

For example, the following code sets the dynamic shapes for an example graph context, specifies the output shape, and updates the context’s required workspace size.

```
var inputShape: [UInt64] = [1024, 1, 1]
let rank = inputShape.count
var outputShape = [UInt64](repeating: 0, count: rank)

let result = outputShape.withUnsafeMutableBufferPointer { output in
    inputShape.withUnsafeMutableBufferPointer { input in

        var shapes = [
            bnns_graph_shape_t(rank: rank, shape: output.baseAddress!),
            bnns_graph_shape_t(rank:rank, shape: input.baseAddress!)
        ]

        return BNNSGraphContextSetDynamicShapes(context, nil,
                                                shapes.count, &shapes)
    }
}

// Prints "[1024, 1, 1]".
print(outputShape)
```

On return, the output shape contains the correct size for the input shape, and a subsequent call to BNNSGraphContextGetWorkspaceSize(_:_:) returns the correct workspace size.

## See Also

### Specifying and querying a context’s properties

func BNNSGraphContextSetArgumentType(bnns_graph_context_t, BNNSGraphArgumentType) -> Int32

Specifies the argument type for a graph context.

struct BNNSGraphArgumentType

Constants that specify the argument type for a graph context.

struct bnns_graph_shape_t

The specification of the shape of an argument.

func BNNSGraphContextSetBatchSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?, UInt64) -> Int32

Sets the batch size for a graph.

func BNNSGraphContextEnableNanAndInfChecks(bnns_graph_context_t, Bool)

Specifies that the context checks intermediate tensors for NaNs and infinities.

func BNNSGraphContextGetWorkspaceSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?) -> Int

Returns the minimum size, in bytes, of the workspace that graph context execution requires.

