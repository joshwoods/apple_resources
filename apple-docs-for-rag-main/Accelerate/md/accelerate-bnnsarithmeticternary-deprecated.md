

- Accelerate
-  BNNSArithmeticTernary Deprecated

Structure

# BNNSArithmeticTernary

A structure that contains the inputs and output of an arithmetic operation with three inputs.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSArithmeticTernary
```

Deprecated

Use BNNSGraph\* APIs

## Overview

Use a BNNSArithmeticTernary structure to pass the descriptions and types of the inputs and output of a binary arithmetic operation to BNNSLayerParametersArithmetic.

The following code shows how to calculate the element-wise multiply-add of two vectors:

```
static func ternaryArithmetic() {

    let aData = UnsafeMutableBufferPointer.allocate(capacity: 1)
    _ = aData.initialize(from: [10])
    let aDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                            layout: BNNSDataLayoutVector,
                                            size: (1, 0, 0, 0, 0, 0, 0, 0),
                                            stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                            data: aData.baseAddress!,
                                            data_type: BNNSDataType.float,
                                            table_data: nil,
                                            table_data_type: BNNSDataType.float,
                                            data_scale: 1, data_bias: 0)

    let bData = UnsafeMutableBufferPointer.allocate(capacity: 1)
    _ = bData.initialize(from: [20])
    let bDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                            layout: BNNSDataLayoutVector,
                                            size: (1, 0, 0, 0, 0, 0, 0, 0),
                                            stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                            data: bData.baseAddress!,
                                            data_type: BNNSDataType.float,
                                            table_data: nil,
                                            table_data_type: BNNSDataType.float,
                                            data_scale: 1, data_bias: 0)

    let cData = UnsafeMutableBufferPointer.allocate(capacity: 1)
    _ = cData.initialize(from: [100])
    let cDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                            layout: BNNSDataLayoutVector,
                                            size: (1, 0, 0, 0, 0, 0, 0, 0),
                                            stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                            data: cData.baseAddress!,
                                            data_type: BNNSDataType.float,
                                            table_data: nil,
                                            table_data_type: BNNSDataType.float,
                                            data_scale: 1, data_bias: 0)

    let outputData = UnsafeMutableBufferPointer.allocate(capacity: 1)
    let outputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                 layout: BNNSDataLayoutVector,
                                                 size: (1, 0, 0, 0, 0, 0, 0, 0),
                                                 stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                 data: outputData.baseAddress!,
                                                 data_type: BNNSDataType.float,
                                                 table_data: nil,
                                                 table_data_type: BNNSDataType.float,
                                                 data_scale: 1, data_bias: 0)

    let fields = BNNSArithmeticTernary(in1: aDescriptor, in1_type: BNNSSample,
                                       in2: bDescriptor, in2_type: BNNSSample,
                                       in3: cDescriptor, in3_type: BNNSSample,
                                       out: outputDescriptor, out_type: BNNSSample)

    let arithmeticLayer: BNNSFilter? = withUnsafePointer(to: fields) { fieldsPtr in

        var layerParameters = BNNSLayerParametersArithmetic(
            arithmetic_function: BNNSArithmeticMultiplyAdd,
            arithmetic_function_fields: UnsafeMutableRawPointer(mutating: fieldsPtr),
            activation: .identity)

        return BNNSFilterCreateLayerArithmetic(&layerParameters, nil)
    }

    var rawInputPointer = [ UnsafeRawPointer(aDescriptor.data!),
                            UnsafeRawPointer(bDescriptor.data!),
                            UnsafeRawPointer(cDescriptor.data!)]

    BNNSArithmeticFilterApplyBatch(arithmeticLayer,
                                   1,
                                   3,
                                   &rawInputPointer,
                                   [1, 1, 1],
                                   outputDescriptor.data!,
                                   1)

    // Prints `10 * 20 + 100 (300)`
    print(Array(outputData))

    aData.deallocate()
    bData.deallocate()
    cData.deallocate()
    outputData.deallocate()
}
```

## Topics

### Creating an Arithmetic Structure

init(in1: BNNSNDArrayDescriptor, in1_type: BNNSDescriptorType, in2: BNNSNDArrayDescriptor, in2_type: BNNSDescriptorType, in3: BNNSNDArrayDescriptor, in3_type: BNNSDescriptorType, out: BNNSNDArrayDescriptor, out_type: BNNSDescriptorType)

Returns a new arithmetic structure that takes three inputs from the specified parameters.

init()

Returns a new arithmetic structure that takes three inputs.

### Inspecting the Properties of an Arithmetic Structure

var in1: BNNSNDArrayDescriptor

The descriptor of the first input.

var in1_type: BNNSDescriptorType

The descriptor type of the first input.

var in2: BNNSNDArrayDescriptor

The descriptor of the second input.

var in2_type: BNNSDescriptorType

The descriptor type of the second input.

var in3: BNNSNDArrayDescriptor

The descriptor of the third input.

var in3_type: BNNSDescriptorType

The descriptor type of the third input.

var out: BNNSNDArrayDescriptor

The descriptor of the output.

var out_type: BNNSDescriptorType

The descriptor type of the output.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Arithmetic layers

class UnaryArithmeticLayer

A layer object that wraps a unary arithmetic filter and manages its deinitialization.

Deprecated

class BinaryArithmeticLayer

A layer object that wraps a binary arithmetic filter and manages its deinitialization.

Deprecated

class TernaryArithmeticLayer

A layer object that wraps a ternary arithmetic filter and manages its deinitialization.

Deprecated

struct BNNSDescriptorType

Constants that describe the input and output types of an arithmetic operation.

struct BNNSArithmeticUnary

A structure that contains the input and output of an arithmetic operation with a single input.

Deprecated

struct BNNSArithmeticBinary

A structure that contains the inputs and output of an arithmetic operation with two inputs.

Deprecated

struct BNNSArithmeticFunction

Constants that define arithmetic operations.

struct BNNSLayerParametersArithmetic

A structure that contains the parameters of an arithmetic layer.

Deprecated

func BNNSFilterCreateLayerArithmetic(UnsafePointer&lt;BNNSLayerParametersArithmetic>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new arithmetic layer.

Deprecated

func BNNSArithmeticFilterApplyBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;Int>, UnsafeMutableRawPointer, Int) -> Int32

Applies an arithmetic filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSArithmeticFilterApplyBackwardBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer?>?, UnsafePointer&lt;Int>?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafePointer&lt;Int>, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies an arithmetic filter backward to generate input gradients.

Deprecated

