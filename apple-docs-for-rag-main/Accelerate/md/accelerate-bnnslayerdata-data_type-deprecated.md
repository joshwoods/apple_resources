

- Accelerate
- BNNSLayerData
-  data_type Deprecated

Instance Property

# data_type

Storage data type for the values stored in data.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
var data_type: BNNSDataType
```

Deprecated

BNNS switched to new Layer Parameters data structures

## See Also

### Instance Properties

var data: UnsafeRawPointer?

Pointer to layer values (weights, bias), layout and size are specific to each layer.

Deprecated

var data_bias: Float

Conversion bias for values, used for integer data types only, ignored for indexed and float data types.

Deprecated

var data_scale: Float

Conversion scale for values, used for integer data types only, ignored for indexed and float data types.

Deprecated

var data_table: UnsafePointer&lt;Float>?

Conversion table (256 values) for indexed floating point data, used for indexed data types only.

Deprecated

