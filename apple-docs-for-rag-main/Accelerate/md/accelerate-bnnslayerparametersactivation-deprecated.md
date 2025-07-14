

- Accelerate
-  BNNSLayerParametersActivation Deprecated

Structure

# BNNSLayerParametersActivation

A set of parameters that define an activation layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersActivation
```

Deprecated

Use BNNSGraph\* APIs

## Overview

Use an activation layer to perform type conversion. The following code shows how to convert 16-bit integer values to single-precision values:

```
let input: [Int16] = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
var output = [Float](repeating: 0, count: input.count)

input.withUnsafeBufferPointer { inputPtr in
    output.withUnsafeMutableBufferPointer { outputPtr in

        let inputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                    layout: BNNSDataLayoutVector,
                                                    size: (input.count, 0, 0, 0, 0, 0, 0, 0),
                                                    stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                    data: UnsafeMutableRawPointer(mutating: inputPtr.baseAddress),
                                                    data_type: .int16,
                                                    table_data: nil,
                                                    table_data_type: .int16,
                                                    data_scale: 1,
                                                    data_bias: 0)

        let ouputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                    layout: BNNSDataLayoutVector,
                                                    size: (input.count, 0, 0, 0, 0, 0, 0, 0),
                                                    stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                    data: outputPtr.baseAddress,
                                                    data_type: .float,
                                                    table_data: nil,
                                                    table_data_type: .float,
                                                    data_scale: 1,
                                                    data_bias: 0)

        var layerParameters = BNNSLayerParametersActivation(i_desc: inputDescriptor,
                                                                 o_desc: ouputDescriptor,
                                                                 activation: .identity,
                                                                 axis_flags: 0)

        BNNSDirectApplyActivationBatch(&layerParameters,
                                       nil,
                                       1,
                                       input.count,
                                       input.count)
    }
}

// Prints "[1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0, 10.0]"
print(output)
```

## Topics

### Initializers

init()

Returns a new activation layer parameters structure.

init(i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, activation: BNNSActivation, axis_flags: UInt32)

Returns a new activation layer parameters structure from the supplied descriptors, activation function, and axis flags.

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var activation: BNNSActivation

The activation function that the layer applies to the output.

var axis_flags: UInt32

Flags that indicate axes on which to apply certain activation functions.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Activation layers

func BNNSFilterCreateVectorActivationLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?Deprecated

class ActivationLayer

A layer object that wraps an activation filter and manages its deinitialization.

Deprecated

struct BNNSActivationFunction

Constants that describe activation functions.

struct BNNSActivation

A set of parameters that describe common activation functions.

func BNNSFilterCreateLayerActivation(UnsafePointer&lt;BNNSLayerParametersActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new activation layer.

Deprecated

func BNNSDirectApplyActivationBatch(UnsafePointer&lt;BNNSLayerParametersActivation>, UnsafePointer&lt;BNNSFilterParameters>?, Int, Int, Int) -> Int32

Applies an activation filter to a set of input objects, writing out the result to a set of output objects.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, axes: [Int], input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies an activation function on the specified axes.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies the specified activation function.

Deprecated

