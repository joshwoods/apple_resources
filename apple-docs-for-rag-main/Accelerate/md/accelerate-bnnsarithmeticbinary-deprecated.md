

- Accelerate
-  BNNSArithmeticBinary Deprecated

Structure

# BNNSArithmeticBinary

A structure that contains the inputs and output of an arithmetic operation with two inputs.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSArithmeticBinary
```

Deprecated

Use BNNSGraph\* APIs

## Overview

Use a BNNSArithmeticUnary structure to pass the descriptions and types of the inputs and output of a binary arithmetic operation to BNNSLayerParametersArithmetic.

The following code shows how to calculate the element-wise sums of two vectors:

```
let inputOne: [Float] = [ 1,  2,  3,  4,  5,  6,  7,  8,  9,  10]
let inputTwo: [Float] = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]
let count = inputOne.count
var outputs = [Float](repeating: 0,
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

var fields = BNNSArithmeticBinary(in1: descriptor, in1_type: BNNSSample,
                                  in2: descriptor, in2_type: BNNSConstant,
                                  out: descriptor, out_type: BNNSSample)

let function = BNNSArithmeticAdd

withUnsafeMutableBytes(of: &fields) { fieldsPtr in

    var layerParameters = BNNSLayerParametersArithmetic(arithmetic_function: function,
                                                        arithmetic_function_fields: fieldsPtr.baseAddress!,
                                                        activation: .identity)

    guard let arithmeticLayer = BNNSFilterCreateLayerArithmetic(&layerParameters, nil) else {
        print("Binary BNNSFilterCreateLayerArithmetic returned nil")
        return
    }
    defer {
        BNNSFilterDestroy(arithmeticLayer)
    }

    inputOne.withUnsafeBytes { in1Ptr in
        inputTwo.withUnsafeBytes { in2Ptr in

            var input = [in1Ptr.baseAddress!, in2Ptr.baseAddress!]

            let error = BNNSArithmeticFilterApplyBatch(arithmeticLayer,
                                                       1,
                                                       2,
                                                       &input,
                                                       [inputOne.count, inputTwo.count],
                                                       &outputs,
                                                       outputs.count)

            print("BNNSArithmeticFilterApplyBatch: error", error)
        }
    }
}

// Prints "[11.0, 22.0, 33.0, 44.0, 55.0, 66.0, 77.0, 88.0, 99.0, 110.0]"
print("Binary Arithmetic: outputs", outputs)
```

## Topics

### Creating an Arithmetic Structure

init(in1: BNNSNDArrayDescriptor, in1_type: BNNSDescriptorType, in2: BNNSNDArrayDescriptor, in2_type: BNNSDescriptorType, out: BNNSNDArrayDescriptor, out_type: BNNSDescriptorType)

Returns a new arithmetic structure that takes two inputs from the specified parameters.

init()

Returns a new arithmetic structure that takes two inputs.

### Inspecting the Properties of an Arithmetic Structure

var in1: BNNSNDArrayDescriptor

The descriptor of the first input.

var in1_type: BNNSDescriptorType

The descriptor type of the first input.

var in2: BNNSNDArrayDescriptor

The descriptor of the second input.

var in2_type: BNNSDescriptorType

The descriptor type of the second input.

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

