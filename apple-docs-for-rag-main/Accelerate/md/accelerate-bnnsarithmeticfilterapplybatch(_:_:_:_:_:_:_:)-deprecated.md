

- Accelerate
-  BNNSArithmeticFilterApplyBatch(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSArithmeticFilterApplyBatch(\_:\_:\_:\_:\_:\_:\_:)

Applies an arithmetic filter to a set of input objects, writing the result to a set of output objects.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSArithmeticFilterApplyBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ number_of_inputs: Int,
    _ in: UnsafeMutablePointer,
    _ in_stride: UnsafePointer,
    _ out: UnsafeMutableRawPointer,
    _ out_stride: Int
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

The filter to apply.

`batch_size`  

The number of input-output pairs.

`number_of_inputs`  

The number of inputs to the arithmetic operation.

`in`  

Pointer to the input data.

`in_stride`  

Increment, in values, between inputs.

`out`  

Pointer to the output data.

`out_stride`  

Increment, in values, between outputs.

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

func BNNSArithmeticFilterApplyBackwardBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer?>?, UnsafePointer&lt;Int>?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafePointer&lt;Int>, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies an arithmetic filter backward to generate input gradients.

Deprecated

