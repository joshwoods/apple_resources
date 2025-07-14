

- Accelerate
-  BNNSFilterCreateLayerNormalization(\_:\_:\_:) Deprecated

Function

# BNNSFilterCreateLayerNormalization(\_:\_:\_:)

Returns a new normalization layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateLayerNormalization(
    _ normType: BNNSFilterType,
    _ layer_params: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> BNNSFilter?
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`normType`  

The normalization type.

`layer_params`  

Layer parameters.

`filter_params`  

The filter runtime parameters.

## Discussion

Use a normalization loss layer to normalize tensor values, that is, calculate new elements to have a zero mean and a unit standard deviation.

For example, given a three-channel image that contains the following values:

```
let input: [Float] = [1, 2, 3, 4, 5, 6, 7, 8, 9,
                      10, 20, 30, 40, 50, 60, 70, 80, 90,
                      100, 200, 300, 400, 500, 600, 700, 800, 900]
```

The following code normalizes each channel and writes the result to the `output` array:

```
let count = input.count
var output = [Float](repeating: 0,
                     count: count)

let descriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                       layout: BNNSDataLayoutImageCHW,
                                       size: (9, 1, 3, 0, 0, 0, 0, 0),
                                       stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                       data: nil,
                                       data_type: BNNSDataType.float,
                                       table_data: nil,
                                       table_data_type: BNNSDataType.float,
                                       data_scale: 1,
                                       data_bias: 0)

var gamma = [Float](repeating: 1,
                    count: descriptor.size.2)

gamma.withUnsafeMutableBufferPointer { gammaPtr in

    let gammaDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                layout: BNNSDataLayoutVector,
                                                size: (descriptor.size.2, 0, 0, 0, 0, 0, 0, 0),
                                                stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                data: gammaPtr.baseAddress,
                                                data_type: BNNSDataType.float,
                                                table_data: nil,
                                                table_data_type: BNNSDataType.float,
                                                data_scale: 1,
                                                data_bias: 0)

    var layerParameters = BNNSLayerParametersNormalization(i_desc: descriptor,
                                                           o_desc: descriptor,
                                                           beta_desc: BNNSNDArrayDescriptor(),
                                                           gamma_desc: gammaDescriptor,
                                                           moving_mean_desc: BNNSNDArrayDescriptor(),
                                                           moving_variance_desc: BNNSNDArrayDescriptor(),
                                                           momentum: 1,
                                                           epsilon: 0,
                                                           activation: .identity,
                                                           num_groups: 1,
                                                           normalization_axis: 0)

    let filter = BNNSFilterCreateLayerNormalization(BNNSInstanceNorm, &layerParameters, nil)
    defer {
        BNNSFilterDestroy(filter)
    }

    BNNSNormalizationFilterApplyBatch(filter, 1,
                                      input, count,
                                      &output, count,
                                      false)
}
```

On return, the output contains the following values:

```
[-1.549, -1.162, -0.775, -0.387, 0.0, 0.387, 0.775, 1.162, 1.549,
 -1.549, -1.162, -0.775, -0.387, 0.0, 0.387, 0.775, 1.162, 1.549,
 -1.549, -1.162, -0.775, -0.387, 0.0, 0.387, 0.775, 1.162, 1.549]
```

## See Also

### Normalization layers

class NormalizationLayer

A layer object that wraps a normalization filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersNormalization

A structure that contains the parameters of a normalization layer.

Deprecated

func BNNSNormalizationFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a normalization filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSNormalizationFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?) -> Int32

Applies a normalization filter backward to generate gradients.

Deprecated

