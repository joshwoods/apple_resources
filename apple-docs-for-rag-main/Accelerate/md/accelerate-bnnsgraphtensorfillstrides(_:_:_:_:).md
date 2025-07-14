

- Accelerate
-  BNNSGraphTensorFillStrides(\_:\_:\_:\_:) 

Function

# BNNSGraphTensorFillStrides(\_:\_:\_:\_:)

Sets the stride of the specifed tensor for compatibility with the given model’s input or output argument based on its current shape.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphTensorFillStrides(
    _ graph: bnns_graph_t,
    _ function: UnsafePointer?,
    _ argument: UnsafePointer,
    _ tensor: UnsafeMutablePointer
) -> Int32
```

## Parameters 

`graph`  

The compiled graph object.

`function`  

The function. Specify as `nil` if the graph only contains one function.

`argument`  

The name of the input or output argument.

`tensor`  

The tensor. On output, the first rank elements contain the strides that BNNS requires.

## Return Value

`0` on success, nonzero on failure.

## Discussion

Call this function to fill the strides of a buffer according to the specification of the compiled graph’s model.

This function requires that you specify the tensor’s sizes. That is, they aren’t less than zero.

## See Also

### Specifying and querying a tensor’s properties

struct BNNSTensor

A structure that describes the shape, stride, data type, and, optionally, the memory location of an n-dimensional array.

func BNNSTensorGetAllocationSize(UnsafePointer&lt;BNNSTensor>) -> Int

Returns the minimum allocation size, in bytes, of the specified tensor.

func BNNSGraphContextGetTensor(bnns_graph_context_t, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>, Bool, UnsafeMutablePointer&lt;BNNSTensor>) -> Int32

Sets the properties of a tensor for the specified function argument.

