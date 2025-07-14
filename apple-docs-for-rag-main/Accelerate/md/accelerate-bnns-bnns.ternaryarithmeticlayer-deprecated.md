

- Accelerate
- BNNS
-  BNNS.TernaryArithmeticLayer Deprecated

Class

# BNNS.TernaryArithmeticLayer

A layer object that wraps a ternary arithmetic filter and manages its deinitialization.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+Mac Catalyst

``` source
class TernaryArithmeticLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Ternary Arithmetic Layer

convenience init?(inputA: BNNSNDArrayDescriptor, inputADescriptorType: BNNS.DescriptorType, inputB: BNNSNDArrayDescriptor, inputBDescriptorType: BNNS.DescriptorType, inputC: BNNSNDArrayDescriptor, inputCDescriptorType: BNNS.DescriptorType, output: BNNSNDArrayDescriptor, outputDescriptorType: BNNS.DescriptorType, function: BNNS.ArithmeticTernaryFunction, activation: BNNS.ActivationFunction, filterParameters: BNNSFilterParameters?)

Returns a new ternary arithmetic layer.

### Specifying a Ternary Arithmetic Function

enum ArithmeticTernaryFunction

Constants that describe ternary arithmetic functions.

### Specifying a Descriptor Type

enum DescriptorType

Constants that describe the input and output types of an arithmetic operation.

### Applying a Ternary Arithmetic Layer

func apply(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, inputC: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor) throws

Applies the layer to a set of input array descriptors, writing the result to a set of output array descriptors.

func applyBackward(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, inputC: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputAGradient: BNNSNDArrayDescriptor, generatingInputBGradient: BNNSNDArrayDescriptor, generatingInputCGradient: BNNSNDArrayDescriptor) throws

Applies the layer backward to generate input gradients.

## Relationships

### Inherits From

- BNNS.Layer

## See Also

### Arithmetic layers

class UnaryArithmeticLayer

A layer object that wraps a unary arithmetic filter and manages its deinitialization.

Deprecated

class BinaryArithmeticLayer

A layer object that wraps a binary arithmetic filter and manages its deinitialization.

Deprecated

struct BNNSDescriptorType

Constants that describe the input and output types of an arithmetic operation.

struct BNNSArithmeticUnary

A structure that contains the input and output of an arithmetic operation with a single input.

Deprecated

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

