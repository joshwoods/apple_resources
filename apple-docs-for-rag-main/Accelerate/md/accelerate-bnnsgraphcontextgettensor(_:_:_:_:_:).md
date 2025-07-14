

- Accelerate
-  BNNSGraphContextGetTensor(\_:\_:\_:\_:\_:) 

Function

# BNNSGraphContextGetTensor(\_:\_:\_:\_:\_:)

Sets the properties of a tensor for the specified function argument.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextGetTensor(
    _ context: bnns_graph_context_t,
    _ function: UnsafePointer?,
    _ argument: UnsafePointer,
    _ fill_known_dynamic_shapes: Bool,
    _ tensor: UnsafeMutablePointer
) -> Int32
```

## Parameters 

`context`  

The graph context.

`function`  

The function. Specify as `nil` if the graph only contains one function.

`argument`  

The name of the input or output argument.

`fill_known_dynamic_shapes`  

A Boolean value that specifies whether the function should replace any dynamic shapes for the next execution of the context. BNNS derives these shapes either from the default shapes in the source model, or from a preceding calls to BNNSGraphContextSetDynamicShapes(_:_:_:_:) or BNNSGraphContextSetBatchSize(_:_:_:). If BNNS is unable to derive the shapes, the function sets the dimensions to `-1`.

`tensor`  

The tensor. On output, all fields apart from data contain the properties for the specified function argument.

## Return Value

`0` on success, nonzero on failure.

## See Also

### Specifying and querying a tensor’s properties

struct BNNSTensor

A structure that describes the shape, stride, data type, and, optionally, the memory location of an n-dimensional array.

func BNNSTensorGetAllocationSize(UnsafePointer&lt;BNNSTensor>) -> Int

Returns the minimum allocation size, in bytes, of the specified tensor.

func BNNSGraphTensorFillStrides(bnns_graph_t, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;BNNSTensor>) -> Int32

Sets the stride of the specifed tensor for compatibility with the given model’s input or output argument based on its current shape.

