

- Accelerate
-  BNNSFilterCreateFusedLayer(\_:\_:\_:\_:) Deprecated

Function

# BNNSFilterCreateFusedLayer(\_:\_:\_:\_:)

Returns a new fused layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateFusedLayer(
    _ number_of_fused_filters: Int,
    _ filter_type: UnsafePointer,
    _ layer_params: UnsafeMutablePointer,
    _ filter_params: UnsafePointer?
) -> BNNSFilter?
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`number_of_fused_filters`  

The number of fused filters.

`filter_type`  

Array of fused filter types.

`layer_params`  

Array of fused layer parameter pointers.

`filter_params`  

The filter runtime parameters.

## Discussion

Use this function to create an `N` layer fused filter that processes input as: `input → filter0 → filter1 →` … `→ filter N-1 → output`. The first `N - 1` filters must have BNNSActivationFunctionIdentity activation function. For the first `N - 2` filters, each filter’s output descriptor and its subsequent filter’s input descriptor must have the same size, stride, and data type.

BNNSFilterCreateFusedLayer(_:_:_:_:) supports two filters. The first filter must be either BNNSConvolution or BNNSFullyConnected. The second filter must be one of BNNSBatchNorm, BNNSInstanceNorm, BNNSLayerNorm, or BNNSGroupNorm.

The following code shows how you pass BNNSLayerParametersConvolution and BNNSLayerParametersNormalization structures to BNNSFilterCreateFusedLayer(_:_:_:_:) to create a fused convolution-layer normalization filter:

```
// `input`, `output`, and `weights` are single-precision arrays.
// `inDescriptor` and `outDescriptor` are the `BNNSNDArrayDescriptor` structures
// for the fused layer's input and output.

weights.withUnsafeMutableBytes { weightsPtr in
    let weightsDescriptor = BNNSNDArrayDescriptor(flags: flags,
                                                  layout: BNNSDataLayoutConvolutionWeightsOIHW,
                                                  size: (3, 3, 1, 1, 0, 0, 0, 0),
                                                  stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                  data: weightsPtr.baseAddress,
                                                  data_type: .float,
                                                  table_data: nil,
                                                  table_data_type: .float,
                                                  data_scale: 0,
                                                  data_bias: 0)

    let convolutionParameters = BNNSLayerParametersConvolution(i_desc: inDescriptor,
                                                               w_desc: weightsDescriptor,
                                                               o_desc: outDescriptor,
                                                               bias: BNNSNDArrayDescriptor(),
                                                               activation: .identity,
                                                               x_stride: 1, y_stride: 1,
                                                               x_dilation_stride: 0, y_dilation_stride: 0,
                                                               x_padding: 0, y_padding: 0,
                                                               groups: 1,
                                                               pad: (0, 0, 0, 0))

    let normalizationParameters = BNNSLayerParametersNormalization(i_desc: outDescriptor,
                                                                   o_desc: outDescriptor,
                                                                   beta_desc: inDescriptor,
                                                                   gamma_desc: inDescriptor,
                                                                   moving_mean_desc: BNNSNDArrayDescriptor(),
                                                                   moving_variance_desc: BNNSNDArrayDescriptor(),
                                                                   momentum: 0,
                                                                   epsilon: 1,
                                                                   activation: .identity,
                                                                   num_groups: 1,
                                                                   normalization_axis: 0)
    withUnsafeBytes(of: convolutionParameters) { convolutionPtr in
        withUnsafeBytes(of: normalizationParameters) { normalizationPtr in

            var parameters = [convolutionPtr.baseAddress!, normalizationPtr.baseAddress!]
            let filter = BNNSFilterCreateFusedLayer(2,
                                                    [BNNSConvolution, BNNSLayerNorm],
                                                    &parameters,
                                                    nil)
            defer {
                BNNSFilterDestroy(filter)
            }

            BNNSFusedFilterApplyBatch(filter, 1,
                                      input, input.count,
                                      &output, output.count,
                                      false)
        }
    }
}
```

## See Also

### Fused layers

protocol FusableLayerParametersDeprecated

class FusedParametersLayer

A layer object that wraps a fused layer and manages its deinitialization.

Deprecated

class FusedConvolutionNormalizationLayer

A layer object that wraps a fused, convolution normalization layer and manages its deinitialization.

Deprecated

class FusedFullyConnectedNormalizationLayer

A layer object that wraps a fused, fully connected normalization layer and manages its deinitialization.

Deprecated

struct BNNSFilterType

Constants that define the component filters of a fused layer.

func BNNSFusedFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a fused filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFusedFilterApplyMultiInputBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;Int>, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a multiple-input fused filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFusedFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?) -> Int32

Applies a fused filter backward to generate input gradients.

Deprecated

func BNNSFusedFilterApplyBackwardMultiInputBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer?>?, UnsafePointer&lt;Int>?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafePointer&lt;Int>, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?) -> Int32

Applies a multiple-input fused filter backward to generate input gradients.

Deprecated

