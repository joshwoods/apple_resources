

- Accelerate
-  BNNSDirectApplyQuantizer(\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSDirectApplyQuantizer(\_:\_:\_:\_:\_:)

Applies a quantization layer directly to two input matrices.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
func BNNSDirectApplyQuantizer(
    _ layer_params: UnsafePointer,
    _ filter_params: UnsafePointer?,
    _ batch_size: Int,
    _ input_stride: Int,
    _ output_stride: Int
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`layer_params`  

The layer parameters.

`filter_params`  

The filter runtime parameters.

`batch_size`  

The number of input-output pairs.

`input_stride`  

The increment, in values, between inputs.

`output_stride`  

The increment, in values, between outputs.

## Discussion

Use this function, in conjunction with a BNNSLayerParametersQuantization, to convert tensors to different precisions. Pass the BNNSQuantizerFunctionQuantize quantizer function to convert a higher-precsion tensor to a lower-precision tensor. Pass BNNSQuantizerFunctionDequantize to convert a lower-precsion tensor to a higher-precision tensor.

Quantization supports the following conversions:

| Source | Destination |
|----|----|
| `BNNSDataTypeInt32`  `BNNSDataTypeFloat16`  `BNNSDataTypeFloat32` | `BNNSDataTypeInt8`  `BNNSDataTypeUInt8`  `BNNSDataTypeInt16`  `BNNSDataTypeUInt16`  `BNNSDataTypeInt32`  `BNNSDataTypeUInt32` |

Dequantization supports the following conversions:

| Source | Destination |
|----|----|
| `BNNSDataTypeInt8`  `BNNSDataTypeUInt8`  `BNNSDataTypeInt16`  `BNNSDataTypeUInt16`  `BNNSDataTypeInt32`  `BNNSDataTypeUInt32` | `BNNSDataTypeInt32`  `BNNSDataTypeFloat16`  `BNNSDataTypeFloat32` |

You can provide optional scale and bias that the function applies during conversion. Quantization returns `y = scale*x + bias`, and dequantization returns `y = (x-bias)/scale`.

If you supply scale and bias descriptors, they must have a vector layout and a size that matches the size of the axis that you specify. If you’re applying scale and bias to the entire tensor, scale and bias descriptors must have a size of 1.

See BNNSQuantizerFunctionDequantize and BNNSQuantizerFunctionQuantize for examples of using this function.

## See Also

### Quantization functions

static func quantize(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int?, scale: BNNSNDArrayDescriptor?, bias: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Quantizes the input tensor and writes the result to the output tensor.

Deprecated

static func dequantize(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int?, scale: BNNSNDArrayDescriptor?, bias: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Dequantizes the input tensor and writes the result to the output tensor.

Deprecated

struct BNNSQuantizerFunction

Constants that describe quantization functions.

struct BNNSLayerParametersQuantization

A structure that contains the parameters of a quantization layer.

Deprecated

