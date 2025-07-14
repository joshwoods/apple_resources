

- Accelerate
- BNNSNDArrayDescriptor
-  data_scale 

Instance Property

# data_scale

The scale you use to convert integer and unsigned integer data to floating point.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var data_scale: Float
```

## See Also

### Accessing the Properties of an Array Descriptor

var flags: BNNSNDArrayFlags

Flags that control some behaviors of the n-dimensional array.

var layout: BNNSDataLayout

The dimension of the n-dimensional array.

var size: (Int, Int, Int, Int, Int, Int, Int, Int)

The number of values in each dimension.

var stride: (Int, Int, Int, Int, Int, Int, Int, Int)

The increment, in values, between consecutive elements in each dimension.

var data: UnsafeMutableRawPointer?

A pointer that is optional and points to the underlying data.

var data_type: BNNSDataType

The data type of the n-dimensional array.

var table_data: UnsafeMutableRawPointer?

The lookup table for indexed data types.

var table_data_type: BNNSDataType

The data type of the lookup table.

var data_bias: Float

The bias you use to convert integer and unsigned integer data to floating point.

var shape: BNNS.Shape

The shape of the n-dimensional array.

