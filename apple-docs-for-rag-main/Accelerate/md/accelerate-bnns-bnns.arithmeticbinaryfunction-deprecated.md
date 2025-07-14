

- Accelerate
- BNNS
-  BNNS.ArithmeticBinaryFunction Deprecated

Enumeration

# BNNS.ArithmeticBinaryFunction

Constants that describe binary arithmetic functions.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
enum ArithmeticBinaryFunction
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Binary Arithmetic Functions

case add

An operation that calculates the element-wise sum of its two inputs.

case subtract

An operation that calculates the element-wise difference of its two inputs.

case divide

An operation that calculates the element-wise division of its two inputs.

case divideNoNaN

An operation that calculates the element-wise division of its two inputs and returns zero if the second input is zero.

case multiply

An operation that calculates the element-wise product of its two inputs.

case multiplyNoNaN

An operation that calculates the element-wise product of its two inputs and returns zero if the second input is zero, even if the first input is NaN or infinity.

case pow

An operation that calculates the element-wise first input raised to the power of its second input.

case max

An operation that calculates the element-wise maximum of its two inputs.

case min

An operation that calculates the element-wise minimum of its two inputs.

### Enumeration Cases

case flooringDivide

case truncatingDivide

case truncatingRemainder

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Equatable
- Hashable

