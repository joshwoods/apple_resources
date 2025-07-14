

- Accelerate
-  BNNSArithmeticUnary Deprecated

Structure

# BNNSArithmeticUnary

A structure that contains the input and output of an arithmetic operation with a single input.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSArithmeticUnary
```

Deprecated

Use BNNSGraph\* APIs

## Overview

Use a BNNSArithmeticUnary structure to pass the descriptions and types of the input and output of a unary arithmetic operation to BNNSLayerParametersArithmetic.

The following code shows how to calculate the element-wise square roots of a vector:

```
let input: [Float] = [4, 16, 9, 25, 100]
let count = input.count
var output = [Float](repeating: .nan,
                     count: count)

let descriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                       layout: BNNSDataLayoutVector,
                                       size: (count, 0, 0, 0, 0, 0, 0, 0),
                                       stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                       data: nil,
                                       data_type: .float,
                                       table_data: nil,
                                       table_data_type: .float,
                                       data_scale: 1,
                                       data_bias: 0)

var fields = BNNSArithmeticUnary(in: descriptor,
                                 in_type: BNNSSample,
                                 out: descriptor,
                                 out_type: BNNSSample)

withUnsafeMutablePointer(to: &fields) { fieldsPtr in

    var layerParameters = BNNSLayerParametersArithmetic(arithmetic_function: BNNSArithmeticSquareRoot,
                                                        arithmetic_function_fields: fieldsPtr,
                                                        activation: .identity)

    guard let arithmeticLayer = BNNSFilterCreateLayerArithmetic(&layerParameters, nil) else {
        print("Unary BNNSFilterCreateLayerArithmetic returns nil")
        return
    }
    defer {
        BNNSFilterDestroy(arithmeticLayer)
    }

    input.withUnsafeBytes { inPtr in
        var rawPtr = inPtr.baseAddress!

        BNNSArithmeticFilterApplyBatch(arithmeticLayer, 1, 1,
                                       &rawPtr,
                                       [count],
                                       &output,
                                       count)
    }
}

// Prints "[2.0, 4.0, 3.0, 5.0, 10.0]"
print("Unary Arithmetic: outputs", output)
```

## Topics

### Creating an Arithmetic Structure

init(in: BNNSNDArrayDescriptor, in_type: BNNSDescriptorType, out: BNNSNDArrayDescriptor, out_type: BNNSDescriptorType)

Returns a new arithmetic structure that takes a single input from the specified parameters.

init()

Returns a new arithmetic structure that takes a single input.

### Inspecting the Properties of an Arithmetic Structure

var `in`: BNNSNDArrayDescriptor

The descriptor of the input.

var in_type: BNNSDescriptorType

The descriptor type of the input.

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

struct BNNSArithmeticBinary

A structure that contains the inputs and output of an arithmetic operation with two inputs.

Deprecated

struct BNNSArithmeticTernary

A structure that contains the inputs and output of an arithmetic operation with three inputs.

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

