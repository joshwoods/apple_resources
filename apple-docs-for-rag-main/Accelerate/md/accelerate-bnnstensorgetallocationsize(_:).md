

- Accelerate
-  BNNSTensorGetAllocationSize(\_:) 

Function

# BNNSTensorGetAllocationSize(\_:)

Returns the minimum allocation size, in bytes, of the specified tensor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSTensorGetAllocationSize(_ tensor: UnsafePointer) -> Int
```

## Parameters 

`tensor`  

The tensor.

## Return Value

The minimum allocation size, in bytes, of the specified tensor.

## See Also

### Specifying and querying a tensor’s properties

struct BNNSTensor

A structure that describes the shape, stride, data type, and, optionally, the memory location of an n-dimensional array.

func BNNSGraphContextGetTensor(bnns_graph_context_t, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>, Bool, UnsafeMutablePointer&lt;BNNSTensor>) -> Int32

Sets the properties of a tensor for the specified function argument.

func BNNSGraphTensorFillStrides(bnns_graph_t, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;BNNSTensor>) -> Int32

Sets the stride of the specifed tensor for compatibility with the given model’s input or output argument based on its current shape.

