

- Accelerate
-  BNNSQuantizerFunction 

Structure

# BNNSQuantizerFunction

Constants that describe quantization functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSQuantizerFunction
```

## Topics

### Quantization Functions

init(UInt32)

Creates a new instance with the specified raw value.

init(rawValue: UInt32)

Creates a new instance with the specified raw value.

var rawValue: UInt32

The corresponding value of the raw type.

var BNNSQuantizerFunctionDequantize: BNNSQuantizerFunction

A constant that specifes conversion to a higher precision.

var BNNSQuantizerFunctionQuantize: BNNSQuantizerFunction

A constant that specifes conversion to a lower precision.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Quantization functions

static func quantize(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int?, scale: BNNSNDArrayDescriptor?, bias: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Quantizes the input tensor and writes the result to the output tensor.

Deprecated

static func dequantize(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int?, scale: BNNSNDArrayDescriptor?, bias: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Dequantizes the input tensor and writes the result to the output tensor.

Deprecated

struct BNNSLayerParametersQuantization

A structure that contains the parameters of a quantization layer.

Deprecated

func BNNSDirectApplyQuantizer(UnsafePointer&lt;BNNSLayerParametersQuantization>, UnsafePointer&lt;BNNSFilterParameters>?, Int, Int, Int) -> Int32

Applies a quantization layer directly to two input matrices.

Deprecated

