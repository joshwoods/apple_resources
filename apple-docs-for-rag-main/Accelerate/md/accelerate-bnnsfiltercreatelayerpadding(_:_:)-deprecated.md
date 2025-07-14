

- Accelerate
-  BNNSFilterCreateLayerPadding(\_:\_:) Deprecated

Function

# BNNSFilterCreateLayerPadding(\_:\_:)

Returns a new loss layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateLayerPadding(
    _ layer_params: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> BNNSFilter?
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`layer_params`  

Layer parameters.

`filter_params`  

The filter runtime parameters.

## Discussion

Use a padding layer to add elements to an n-dimensional array before and after existing data. The padding can either contain a single value or a reflection of the existing data. For `BNNSPaddingModeConstant`, pass the bit pattern of the padding value, for example, using bitPattern to pass a single-precision value.

The following code shows how to add two elements before, and four elements after a vector of ten values:

```
let paddingSize = (2, 4)

let source: [Float] = [ 0, 1, 2, 3, 4, 5, 7, 8, 9 ]

var destination = [Float](repeating: 0,
                          count: source.count + paddingSize.0 + paddingSize.1)

let srcDescription = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                           layout: BNNSDataLayoutVector,
                                           size: (source.count, 0, 0, 0, 0, 0, 0, 0),
                                           stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                           data: nil,
                                           data_type: .float,
                                           table_data: nil,
                                           table_data_type: .float,
                                           data_scale: 1,
                                           data_bias: 0)

let destDescription = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                            layout: BNNSDataLayoutVector,
                                            size: (destination.count, 0, 0, 0, 0, 0, 0, 0),
                                            stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                            data: nil,
                                            data_type: .float,
                                            table_data: nil,
                                            table_data_type: .float,
                                            data_scale: 1,
                                            data_bias: 0)

let paddingValue: Float = 99

var parameters = BNNSLayerParametersPadding(i_desc: srcDescription,
                                            o_desc: destDescription,
                                            padding_size: (paddingSize, (0, 0), (0, 0), (0, 0),
                                                           (0, 0), (0, 0), (0, 0), (0, 0)),
                                            padding_mode: BNNSPaddingModeConstant,
                                            padding_value: paddingValue.bitPattern)

var filterParams = BNNSFilterParameters()

let filter = BNNSFilterCreateLayerPadding(&parameters, &filterParams)
defer {
    BNNSFilterDestroy(filter)
}

BNNSFilterApply(filter,
                source,
                &destination)
```

On return, `destination` contains `[99.0, 99.0, 0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 7.0, 8.0, 9.0, 99.0, 99.0, 99.0, 99.0]`.

## See Also

### Padding layers

class PaddingLayer

A layer object that wraps a padding filter and manages its deinitialization.

Deprecated

struct BNNSPaddingMode

Constants that define padding modes.

struct BNNSLayerParametersPadding

A structure that contains the parameters of a padding layer.

Deprecated

