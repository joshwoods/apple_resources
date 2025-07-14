

- Accelerate
- BNNSTensor
-  data_size_in_bytes 

Instance Property

# data_size_in_bytes

The size, in bytes, of the memory that contains the tensor values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var data_size_in_bytes: Int
```

## See Also

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

var name: UnsafePointer&lt;CChar>?

An optional name for the tensor that you can use for debugging.

