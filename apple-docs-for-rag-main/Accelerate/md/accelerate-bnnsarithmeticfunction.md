

- Accelerate
-  BNNSArithmeticFunction 

Structure

# BNNSArithmeticFunction

Constants that define arithmetic operations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSArithmeticFunction
```

## Topics

### Unary Arithmetic Functions

var BNNSArithmeticCeil: BNNSArithmeticFunction

An operation that calculates the element-wise ceiling of its input.

var BNNSArithmeticFloor: BNNSArithmeticFunction

An operation that calculates the element-wise floor of its input.

var BNNSArithmeticSquareRoot: BNNSArithmeticFunction

An operation that calculates the element-wise square root of its input.

var BNNSArithmeticReciprocalSquareRoot: BNNSArithmeticFunction

An operation that calculates the element-wise reciprocal square root of its input.

var BNNSArithmeticRound: BNNSArithmeticFunction

An operation that calculates the element-wise rounding of its input.

var BNNSArithmeticAbs: BNNSArithmeticFunction

An operation that calculates the element-wise absolute of its input.

var BNNSArithmeticErf: BNNSArithmeticFunction

An operation that calculates the element-wise error function of its input.

var BNNSArithmeticNegate: BNNSArithmeticFunction

An operation that calculates the element-wise negation of its input.

var BNNSArithmeticReciprocal: BNNSArithmeticFunction

An operation that calculates the element-wise reciprocal of its input.

var BNNSArithmeticSign: BNNSArithmeticFunction

An operation that calculates the element-wise sign of its input.

var BNNSArithmeticSquare: BNNSArithmeticFunction

An operation that calculates the element-wise square of its input.

### Binary Arithmetic Functions

var BNNSArithmeticAdd: BNNSArithmeticFunction

An operation that calculates the element-wise sum of its two inputs.

var BNNSArithmeticSubtract: BNNSArithmeticFunction

An operation that calculates the element-wise difference of its two inputs.

var BNNSArithmeticDivide: BNNSArithmeticFunction

An operation that calculates the element-wise division of its two inputs.

var BNNSArithmeticDivideNoNaN: BNNSArithmeticFunction

An operation that calculates the element-wise division of its two inputs and returns zero if the divisor is zero, even if the first input is NaN or infinity.

var BNNSArithmeticMultiply: BNNSArithmeticFunction

An operation that calculates the element-wise product of its two inputs.

var BNNSArithmeticMultiplyNoNaN: BNNSArithmeticFunction

An operation that calculates the element-wise product of its two inputs and returns zero, even if the first input is NaN or infinity.

var BNNSArithmeticPow: BNNSArithmeticFunction

An operation that calculates the element-wise first input raised to the power of its second input.

var BNNSArithmeticMaximum: BNNSArithmeticFunction

An operation that calculates the element-wise maximum of its two inputs.

var BNNSArithmeticMinimum: BNNSArithmeticFunction

An operation that calculates the element-wise minimum of its two inputs.

var BNNSArithmeticFloorDivide: BNNSArithmeticFunction

An operation that calculates the element-wise floor division of its inputs.

var BNNSArithmeticTruncDivide: BNNSArithmeticFunction

An operation that calculates the element-wise truncated division of its inputs.

var BNNSArithmeticTruncRemainder: BNNSArithmeticFunction

An operation that calculates the element-wise remainder of truncated division of its inputs.

### Ternary Arithmetic Functions

var BNNSArithmeticMultiplyAdd: BNNSArithmeticFunction

An operation that calculates the element-wise fused multiply-add of its three inputs.

var BNNSArithmeticSelect: BNNSArithmeticFunction

An operation that selects elements from either its second or third input based on the corresponding value of its first input.

### Exponential and Logarithmic Functions

var BNNSArithmeticExp: BNNSArithmeticFunction

An operation that calculates the element-wise result of *e* raised to the power of its input.

var BNNSArithmeticExp2: BNNSArithmeticFunction

An operation that calculates the element-wise result of 2 raised to the power of its input.

var BNNSArithmeticLog: BNNSArithmeticFunction

An operation that calculates the element-wise natural logarithm of its input.

var BNNSArithmeticLog2: BNNSArithmeticFunction

An operation that calculates the element-wise base 2 logarithm of its input.

### Trigonometric Functions

var BNNSArithmeticAcos: BNNSArithmeticFunction

An operation that calculates the element-wise inverse cosine of its input.

var BNNSArithmeticAcosh: BNNSArithmeticFunction

An operation that calculates the element-wise inverse hyperbolic cosine of its input.

var BNNSArithmeticAsin: BNNSArithmeticFunction

An operation that calculates the element-wise inverse sine of its input.

var BNNSArithmeticAsinh: BNNSArithmeticFunction

An operation that calculates the element-wise inverse hyperbolic sine of its input.

var BNNSArithmeticAtan: BNNSArithmeticFunction

An operation that calculates the element-wise inverse tangent of its input.

var BNNSArithmeticAtanh: BNNSArithmeticFunction

An operation that calculates the element-wise inverse hyperbolic tangent of its input.

var BNNSArithmeticCos: BNNSArithmeticFunction

An operation that calculates the element-wise cosine of its input.

var BNNSArithmeticCosh: BNNSArithmeticFunction

An operation that calculates the element-wise hyperbolic cosine of its input.

var BNNSArithmeticSin: BNNSArithmeticFunction

An operation that calculates the element-wise sine of its input.

var BNNSArithmeticSinh: BNNSArithmeticFunction

An operation that calculates the element-wise hyperbolic sine of its input.

var BNNSArithmeticTan: BNNSArithmeticFunction

An operation that calculates the element-wise tangent of its input.

var BNNSArithmeticTanh: BNNSArithmeticFunction

An operation that calculates the element-wise hyperbolic tangent of its input.

### Raw Values

var rawValue: UInt32

init(UInt32)

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

