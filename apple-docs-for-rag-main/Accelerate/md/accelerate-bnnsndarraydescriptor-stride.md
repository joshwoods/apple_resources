

- Accelerate
- BNNSNDArrayDescriptor
-  stride 

Instance Property

# stride

The increment, in values, between consecutive elements in each dimension.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var stride: (Int, Int, Int, Int, Int, Int, Int, Int)
```

## Discussion

Specify the stride of an array descriptor the define the increment between neighboring elements in each dimension. For example, the following values represent a 2D row-major matrix:

```
[ 10, 20, 30,
  40, 50, 60,
  70, 80, 90 ]
```

The stride for the first dimension is `1`, for example, the increment between `50` and `60` is a single element. The stride for the second dimension is `3`, for example, the stride between `50` and `80` is three elements.

## See Also

### Accessing the Properties of an Array Descriptor

var flags: BNNSNDArrayFlags

Flags that control some behaviors of the n-dimensional array.

var layout: BNNSDataLayout

The dimension of the n-dimensional array.

var size: (Int, Int, Int, Int, Int, Int, Int, Int)

The number of values in each dimension.

var data: UnsafeMutableRawPointer?

A pointer that is optional and points to the underlying data.

var data_type: BNNSDataType

The data type of the n-dimensional array.

var table_data: UnsafeMutableRawPointer?

The lookup table for indexed data types.

var table_data_type: BNNSDataType

The data type of the lookup table.

var data_scale: Float

The scale you use to convert integer and unsigned integer data to floating point.

var data_bias: Float

The bias you use to convert integer and unsigned integer data to floating point.

var shape: BNNS.Shape

The shape of the n-dimensional array.

