

- Accelerate
- BNNSTensor
-  rank 

Instance Property

# rank

The rank of the tensor.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rank: UInt8
```

## Discussion

This value must be greater than or equal to zero, and less than or equal to `BNNS_MAX_TENSOR_DIMENSION`.

## See Also

### Specifying a tensor’s properties

var data_type: BNNSDataType

The data type of the tensor.

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

