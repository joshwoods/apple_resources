

- Accelerate
- BNNS
-  BNNS.UnaryArithmeticLayer Deprecated

Class

# BNNS.UnaryArithmeticLayer

A layer object that wraps a unary arithmetic filter and manages its deinitialization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class UnaryArithmeticLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Unary Arithmetic Layer

convenience init?(input: BNNSNDArrayDescriptor, inputDescriptorType: BNNS.DescriptorType, output: BNNSNDArrayDescriptor, outputDescriptorType: BNNS.DescriptorType, function: BNNS.ArithmeticUnaryFunction, activation: BNNS.ActivationFunction, filterParameters: BNNSFilterParameters?)

Returns a new unary arithmetic layer.

### Specifying a Unary Arithmetic Function

enum ArithmeticUnaryFunction

Constants that describe unary arithmetic functions.

### Specifying a Descriptor Type

enum DescriptorType

Constants that describe the input and output types of an arithmetic operation.

### Applying a Unary Arithmetic Layer

func apply(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

func applyBackward(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor) throws

Applies the layer backward to generate input gradients.

## Relationships

### Inherits From

- BNNS.Layer

## See Also

### Arithmetic layers

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

