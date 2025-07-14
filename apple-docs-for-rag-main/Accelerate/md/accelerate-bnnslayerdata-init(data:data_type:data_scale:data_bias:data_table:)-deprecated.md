

- Accelerate
- BNNSLayerData
-  init(data:data_type:data_scale:data_bias:data_table:) Deprecated

Initializer

# init(data:data_type:data_scale:data_bias:data_table:)

Returns a new layer data structure.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
init(
    data: UnsafeRawPointer?,
    data_type: BNNSDataType,
    data_scale: Float,
    data_bias: Float,
    data_table: UnsafePointer?
)
```

Deprecated

BNNS switched to new Layer Parameters data structures

## Parameters 

`data`  

Pointer to layer values (weights, bias), layout and size are specific to each layer.

`data_type`  

Storage data type for the values stored in data.

`data_scale`  

Conversion scale for values, used for integer data types only, ignored for indexed and float data types.

`data_bias`  

Conversion bias for values, used for integer data types only, ignored for indexed and float data types.

`data_table`  

Conversion table (256 values) for indexed floating point data, used for indexed data types only.

## Return Value

A new layer data structure.

## See Also

### Initializers

init()Deprecated

init(data: UnsafeRawPointer?, data_type: BNNSDataType, data_scale: Float, data_bias: Float)Deprecated

