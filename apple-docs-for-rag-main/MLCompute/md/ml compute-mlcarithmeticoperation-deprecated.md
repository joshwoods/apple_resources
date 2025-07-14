

- ML Compute
-  MLCArithmeticOperation Deprecated

Enumeration

# MLCArithmeticOperation

Constants that describe an arithmetic operation.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
enum MLCArithmeticOperation
```

## Topics

### Basic Operations

case add

Calculates the element-wise sum of the inputs.

case subtract

Calculates the element-wise difference between the inputs.

case multiply

Calculates the element-wise product of the inputs.

case multiplyNoNaN

Calculates the element-wise product of the inputs, and returns `0` when the result isn’t a number or infinity.

case divide

Calculates the element-wise division of the inputs.

case divideNoNaN

Calculates the element-wise division of the inputs, and returns `0` if the denominator is `0`.

case min

Calculates the element-wise minimum of the inputs.

case max

Calculates the element-wise maximum the inputs.

### Rounding Operations

case floor

Calculates the element-wise floor of the inputs.

case round

Calculates the element-wise rounding of the inputs.

case ceil

Calculates the element-wise ceiling of the inputs.

### Trigonometric Operations

case sin

Calculates the element-wise sine of the input.

case cos

Calculates the element-wise cosine of the input.

case tan

Calculates the element-wise tangent of the input.

case asin

Calculates the element-wise inverse sine of the input.

case acos

Calculates the element-wise inverse cosine of the input.

case atan

Calculates the element-wise inverse tangent of the input.

case sinh

Calculates the element-wise hyperbolic sine of the input.

case cosh

Calculates the element-wise hyperbolic cosine of the input.

case tanh

Calculates the element-wise hyperbolic tangent of the input.

case asinh

Calculates the element-wise inverse hyperbolic sine of the input.

case acosh

Calculates the element-wise inverse hyperbolic cosine of the input.

case atanh

Calculates the element-wise inverse hyperbolic tangent of the input.

### Advanced Operations

case sqrt

Calculates the element-wise square root of the input.

case rsqrt

Calculates the element-wise reciprocal of the square root of the input.

case pow

Calculates the element-wise first input raised to the power of the second input.

case exp

Calculates the element-wise result of the exponent raised to the power of the input.

case exp2

Calculates the element-wise result of the number 2 raised to the power of the input.

case log

Calculates the element-wise natural logarithm of the input.

case log2

Calculates the element-wise base 2 logarithm of the input.

### Debugging

var debugDescription: String

A textual description of the arithmetic operation you use for debugging.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Arithmetic Layers

convenience init(operation: MLCArithmeticOperation)

Creates an arithmetic layer with the operation you specify.

Deprecated

