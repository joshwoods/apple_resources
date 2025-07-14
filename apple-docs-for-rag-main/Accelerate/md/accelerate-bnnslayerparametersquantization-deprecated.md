

- Accelerate
-  BNNSLayerParametersQuantization Deprecated

Structure

# BNNSLayerParametersQuantization

A structure that contains the parameters of a quantization layer.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
struct BNNSLayerParametersQuantization
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init()

Returns a new quantization layer parameters structure.

init(axis_mask: Int, function: BNNSQuantizerFunction, i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, scale: BNNSNDArrayDescriptor, bias: BNNSNDArrayDescriptor)

Returns a new quantization layer parameters structure using the supplied parameters.

### Instance Properties

var axis_mask: Int

A bitmask that defines the axis to which the function applies scale and bias.

var function: BNNSQuantizerFunction

The quantize function.

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var scale: BNNSNDArrayDescriptor

The descriptor of the scale.

var bias: BNNSNDArrayDescriptor

The descriptor of the bias.

## Relationships

### Conforms To

- BitwiseCopyable

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

func BNNSDirectApplyQuantizer(UnsafePointer&lt;BNNSLayerParametersQuantization>, UnsafePointer&lt;BNNSFilterParameters>?, Int, Int, Int) -> Int32

Applies a quantization layer directly to two input matrices.

Deprecated

