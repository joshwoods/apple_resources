

- Accelerate
-  BNNSFilterCreateLayerTransposedConvolution(\_:\_:) Deprecated

Function

# BNNSFilterCreateLayerTransposedConvolution(\_:\_:)

Returns a new transposed convolution layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateLayerTransposedConvolution(
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

Use transposed convolution to upsample a tensor by performing an operation that’s effectively the inverse of a convolution.

The following figure illustrates the process of transposed convolution. The operation multiplies each element in the input by the kernel to produce the corresponding values in the output. The final output, pictured at the bottom of the figure, is the sum of the products:

Use the following code to perform the illustrated transposed convolution:

```
let input = [Float](repeating: 1, count: 2 * 2)

var kernel = [Float](repeating: 1, count: 3 * 3)

var output = [Float](repeating: 0, count: 4 * 4)

kernel.withUnsafeMutableBufferPointer { kernelPtr in

    let inDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                             layout: BNNSDataLayoutImageCHW,
                                             size: (2, 2, 1, 0, 0, 0, 0, 0),
                                             stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                             data: nil,
                                             data_type: .float,
                                             table_data: nil,
                                             table_data_type: .float,
                                             data_scale: 1,
                                             data_bias: 0)

    let weightsDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                  layout: BNNSDataLayoutConvolutionWeightsOIHW,
                                                  size: (3, 3, 1, 1, 0, 0, 0, 0),
                                                  stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                  data: kernelPtr.baseAddress,
                                                  data_type: .float,
                                                  table_data: nil,
                                                  table_data_type: .float,
                                                  data_scale: 1,
                                                  data_bias: 0)

    let outDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                              layout: BNNSDataLayoutImageCHW,
                                              size: (4, 4, 1, 0, 0, 0, 0, 0),
                                              stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                              data: nil,
                                              data_type: .float,
                                              table_data: nil,
                                              table_data_type: .float,
                                              data_scale: 1,
                                              data_bias: 0)

    var parameters = BNNSLayerParametersConvolution(i_desc: inDescriptor,
                                                    w_desc: weightsDescriptor,
                                                    o_desc: outDescriptor,
                                                    bias: BNNSNDArrayDescriptor(),
                                                    activation: .identity,
                                                    x_stride: 1, y_stride: 1,
                                                    x_dilation_stride: 0, y_dilation_stride: 0,
                                                    x_padding: 0, y_padding: 0,
                                                    groups: 1,
                                                    pad: (0, 0, 0, 0))

    let filter = BNNSFilterCreateLayerTransposedConvolution(&parameters,
                                                            nil)
    defer {
        BNNSFilterDestroy(filter)
    }

    BNNSFilterApply(filter,
                    input,
                    &output)
}
```

On return, `output` contains the following values:

```
[ 1.0, 2.0, 2.0, 1.0, 
  2.0, 4.0, 4.0, 2.0, 
  2.0, 4.0, 4.0, 2.0, 
  1.0, 2.0, 2.0, 1.0 ]
```

## See Also

### Convolution layers

struct BNNSConvolutionLayerParameters

A structure containing convolution parameters.

Deprecated

func BNNSFilterCreateConvolutionLayer(UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSConvolutionLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a convolution filter, initialized with input, output, layer, and filter parameters.

Deprecated

class ConvolutionLayer

A layer object that wraps a convolution filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersConvolution

A structure that contains the parameters of a convolution layer.

Deprecated

func BNNSFilterCreateLayerConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new convolution layer.

Deprecated

