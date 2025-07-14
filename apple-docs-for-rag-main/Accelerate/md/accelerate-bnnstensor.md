

- Accelerate
-  BNNSTensor 

Structure

# BNNSTensor

A structure that describes the shape, stride, data type, and, optionally, the memory location of an n-dimensional array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSTensor
```

## Topics

### Initializers

init()

Creates an empty tensor.

init(data_type: BNNSDataType, rank: UInt8, shape: (Int, Int, Int, Int, Int, Int, Int, Int), stride: (Int, Int, Int, Int, Int, Int, Int, Int), data: UnsafeMutableRawPointer?, data_size_in_bytes: Int, name: UnsafePointer&lt;CChar>?)

Creates a tensor with the specified properties.

### Specifying a tensor’s properties

var data_type: BNNSDataType

The data type of the tensor.

var rank: UInt8

The rank of the tensor.

var shape: (Int, Int, Int, Int, Int, Int, Int, Int)

A tuple of unsigned-integer elements that specify the size of the tensor.

var stride: (Int, Int, Int, Int, Int, Int, Int, Int)

A tuple of unsigned-integer elements that specify the stride of the tensor.

var data: UnsafeMutableRawPointer?

A pointer to the memory that contains the tensor values.

var data_size_in_bytes: Int

The size, in bytes, of the memory that contains the tensor values.

var name: UnsafePointer&lt;CChar>?

An optional name for the tensor that you can use for debugging.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Specifying and querying a tensor’s properties

func BNNSTensorGetAllocationSize(UnsafePointer&lt;BNNSTensor>) -> Int

Returns the minimum allocation size, in bytes, of the specified tensor.

func BNNSGraphContextGetTensor(bnns_graph_context_t, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>, Bool, UnsafeMutablePointer&lt;BNNSTensor>) -> Int32

Sets the properties of a tensor for the specified function argument.

func BNNSGraphTensorFillStrides(bnns_graph_t, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;BNNSTensor>) -> Int32

Sets the stride of the specifed tensor for compatibility with the given model’s input or output argument based on its current shape.

